# 分区和文件系统扩展前准备（Linux）<a name="evs_01_0035"></a>

扩展磁盘分区和文件系统前，请先检查磁盘的分区形式和文件系统，并根据磁盘的分区形式选择对应的操作指导。

1.  检查磁盘分区形式，请参见：
    -   [方法一：查看分区形式和文件系统](#section45741613172812)
    -   [方法二：查看分区形式和文件系统](#section7627683297)

2.  选择操作指导，请参见：[分区和文件系统扩展场景说明](#section1136918160143)。

## 方法一：查看分区形式和文件系统<a name="section45741613172812"></a>

1.  <a name="li4640174163019"></a>执行以下命令，查看云服务器挂载的所有磁盘情况。

    **lsblk**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# lsblk
    NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    vda    253:0    0   40G  0 disk
    └─vda1 253:1    0   40G  0 part /
    vdb    253:16   0  150G  0 disk
    └─vdb1 253:17   0  100G  0 part /mnt/sdc
    ```

    本示例中数据盘“/dev/vdb”扩容前已有分区“/dev/vdb1”，将数据盘扩容50GB后，新增的容量还未划分磁盘分区，因此“/dev/vdb”显示150GB，“/dev/vdb1”显示100GB。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果执行了**lsblk**，发现磁盘“/dev/vdb”没有分区，针对这种没有分区的磁盘，扩容后的容量可能无法正常使用，您也可以通过华为云社区寻找扩展未分区磁盘文件系统的方法。  

2.  执行以下命令，查看当前磁盘分区的分区形式。

    **fdisk -l**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# fdisk -l
    
    Disk /dev/vda: 42.9 GB, 42949672960 bytes, 83886080 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000bcb4e
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    
    Disk /dev/vdb: 161.1 GB, 161061273600 bytes, 314572800 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x38717fc1
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vdb1            2048   209715199   104856576   83  Linux
    ```

    “system”为“Linux”表示分区形式为MBR。“system”为“GPT”表示分区形式为GPT。

    -   若回显中没有列出所有的磁盘分区，和[1](#li4640174163019)中的信息不符合。可能原因是：磁盘已有分区为GPT，并且扩容后存在未分配分区的空间，此时使用**fdisk -l**无法查看所有分区的信息，请参考[方法二：查看分区形式和文件系统](#section7627683297)重新确认磁盘分区形式和文件系统。
    -   若回显中列出了所有的磁盘分区，和[1](#li4640174163019)中的信息符合，则继续执行以下操作。

3.  执行以下命令，查看磁盘分区的文件系统格式。

    **blkid** _磁盘分区_

    命令示例：

    **blkid /dev/vdb1**

    “TYPE”为“ext4”：表示为/dev/vdb1的文件系统是ext4。

4.  执行以下命令，确认文件系统的状态。

    ext\*：**e2fsck -n** _磁盘分区_

    xfs：**xfs\_repair -n** _磁盘分区_

    以“ext4” 为例：

    **e2fsck -n /dev/vdb1**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# e2fsck -n /dev/vdb1
    e2fsck 1.42.9 (28-Dec-2013)
    Warning!  /dev/vdb1 is mounted.
    Warning: skipping journal recovery because doing a read-only filesystem check.
    /dev/vdb1: clean, 11/6553600 files, 459544/26214144 blocks
    ```

    文件系统状态为clean表示状态正常，若不是clean，请先修复问题后执行扩容操作。


## 方法二：查看分区形式和文件系统<a name="section7627683297"></a>

1.  执行以下命令，查看云服务器挂载的所有磁盘情况。

    **lsblk**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# lsblk
    NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    vda    253:0    0   40G  0 disk
    └─vda1 253:1    0   40G  0 part /
    vdb    253:16   0  150G  0 disk
    └─vdb1 253:17   0  100G  0 part /mnt/sdc
    ```

    本示例中数据盘“/dev/vdb”扩容前已有分区“/dev/vdb1”，将数据盘扩容50GB后，新增的容量还未划分磁盘分区，因此“/dev/vdb”显示150GB，“/dev/vdb1”显示100GB。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果执行了**lsblk**，发现磁盘“/dev/vdb”没有分区，针对这种没有分区的磁盘，扩容后的容量可能无法正常使用，您也可以通过华为云社区寻找扩展未分区磁盘文件系统的方法。  

2.  执行以下命令，指定一块磁盘，然后输入“p”，查看磁盘的分区形式。

    **parted** _磁盘_

    以查看“/dev/vdb”的分区形式为例：

    **parted /dev/vdb**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# parted /dev/vdb
    GNU Parted 3.1
    Using /dev/vdb
    Welcome to GNU Parted! Type 'help' to view a list of commands.
    (parted) p
    Error: The backup GPT table is not at the end of the disk, as it should be.  This might mean that another operating system believes the
    disk is smaller.  Fix, by moving the backup to the end (and removing the old backup)?
    Fix/Ignore/Cancel? Fix
    Warning: Not all of the space available to /dev/vdb appears to be used, you can fix the GPT to use all of the space (an extra 104857600
    blocks) or continue with the current setting?
    Fix/Ignore? Fix
    Model: Virtio Block Device (virtblk)
    Disk /dev/vdb: 161GB
    Sector size (logical/physical): 512B/512B
    Partition Table: gpt
    Disk Flags:
    
    Number  Start   End    Size   File system  Name  Flags
     1      1049kB  107GB  107GB  ext4         test
    
    (parted) 
    ```

    “Partition Table”表示当前磁盘的分区形式，msdos表示磁盘分区形式为MBR，gpt表示磁盘分区形式为GPT。

    -   若系统出现以下Error，请输入“Fix”。

        ```
        Error: The backup GPT table is not at the end of the disk, as it should be.  This might mean that another operating system believes the
        disk is smaller.  Fix, by moving the backup to the end (and removing the old backup)?
        ```

        GPT分区表信息存储在磁盘开头，为了减少分区表损坏的风险，同时在磁盘末尾会备份一份。当磁盘容量扩大后，末尾位置也会随之变化，因此需要根据系统提示输入“Fix”，将分区表信息的备份文件挪到新的磁盘末尾位置。

    -   若系统出现以下Warning，请输入“Fix”。

        ```
        Warning: Not all of the space available to /dev/vdb appears to be used, you can fix the GPT to use all of the space (an extra 104857600
        blocks) or continue with the current setting?
        Fix/Ignore? Fix
        ```

        根据系统提示输入“Fix”，系统会自动将磁盘扩容部分的容量设置为GPT。

3.  查看完成后，输入“q”，退出parted模式。

## 分区和文件系统扩展场景说明<a name="section1136918160143"></a>

**表 1**  分区和文件系统扩展场景说明

<a name="table378248191411"></a>
<table><thead align="left"><tr id="row127801589149"><th class="cellrowborder" valign="top" width="9.450945094509452%" id="mcps1.2.6.1.1"><p id="p67805813143"><a name="p67805813143"></a><a name="p67805813143"></a>磁盘</p>
</th>
<th class="cellrowborder" valign="top" width="27.19271927192719%" id="mcps1.2.6.1.2"><p id="p197801817146"><a name="p197801817146"></a><a name="p197801817146"></a>场景</p>
</th>
<th class="cellrowborder" valign="top" width="17.42174217421742%" id="mcps1.2.6.1.3"><p id="p07801289143"><a name="p07801289143"></a><a name="p07801289143"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="13.571357135713571%" id="mcps1.2.6.1.4"><p id="p1278058171417"><a name="p1278058171417"></a><a name="p1278058171417"></a>影响</p>
</th>
<th class="cellrowborder" valign="top" width="32.363236323632364%" id="mcps1.2.6.1.5"><p id="p15780148151415"><a name="p15780148151415"></a><a name="p15780148151415"></a>约束与限制</p>
</th>
</tr>
</thead>
<tbody><tr id="row83901751558"><td class="cellrowborder" rowspan="2" valign="top" width="9.450945094509452%" headers="mcps1.2.6.1.1 "><p id="p1390053558"><a name="p1390053558"></a><a name="p1390053558"></a>系统盘</p>
</td>
<td class="cellrowborder" valign="top" width="27.19271927192719%" headers="mcps1.2.6.1.2 "><p id="p86391164554"><a name="p86391164554"></a><a name="p86391164554"></a>为扩容部分的云硬盘分配新的MBR分区</p>
</td>
<td class="cellrowborder" valign="top" width="17.42174217421742%" headers="mcps1.2.6.1.3 "><p id="p9322120105510"><a name="p9322120105510"></a><a name="p9322120105510"></a><a href="扩展系统盘的分区和文件系统（Linux）.md#section9194153012119">新增MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" width="13.571357135713571%" headers="mcps1.2.6.1.4 "><p id="p730114243555"><a name="p730114243555"></a><a name="p730114243555"></a><a href="#li4674330102614">不中断业务</a></p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="32.363236323632364%" headers="mcps1.2.6.1.5 "><p id="p1058715298558"><a name="p1058715298558"></a><a name="p1058715298558"></a>EVS服务支持的最大系统盘容量为1 TB（1024 GB），即您最大可将系统盘扩容至1 TB。</p>
</td>
</tr>
<tr id="row5723127155520"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p563914165557"><a name="p563914165557"></a><a name="p563914165557"></a>将扩容部分的容量划分至已有的MBR分区内</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p16322220145511"><a name="p16322220145511"></a><a name="p16322220145511"></a><a href="扩展系统盘的分区和文件系统（Linux）.md#section143412109355">扩大已有MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p8302142415518"><a name="p8302142415518"></a><a name="p8302142415518"></a><a href="#li132901912815">依据Linux内核版本决定是否中断业务</a></p>
</td>
</tr>
<tr id="row1378110851412"><td class="cellrowborder" rowspan="4" valign="top" width="9.450945094509452%" headers="mcps1.2.6.1.1 "><p id="p13780384149"><a name="p13780384149"></a><a name="p13780384149"></a>数据盘</p>
</td>
<td class="cellrowborder" valign="top" width="27.19271927192719%" headers="mcps1.2.6.1.2 "><p id="p17807811417"><a name="p17807811417"></a><a name="p17807811417"></a>为扩容部分的云硬盘分配新的MBR分区</p>
</td>
<td class="cellrowborder" valign="top" width="17.42174217421742%" headers="mcps1.2.6.1.3 "><p id="p1378058181415"><a name="p1378058181415"></a><a name="p1378058181415"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section20200028194016">新增MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" width="13.571357135713571%" headers="mcps1.2.6.1.4 "><p id="p278018141414"><a name="p278018141414"></a><a name="p278018141414"></a><a href="#li8782887145">不中断业务</a></p>
</td>
<td class="cellrowborder" rowspan="6" valign="top" width="32.363236323632364%" headers="mcps1.2.6.1.5 "><div class="p" id="p28915510213"><a name="p28915510213"></a><a name="p28915510213"></a>EVS服务支持的最大数据盘容量为32 TB（32768 GB）。<a name="ul899913613126"></a><a name="ul899913613126"></a><ul id="ul899913613126"><li>当数据盘使用MBR分区形式时，容量最大支持2 TB（2048 GB），超过2 TB的部分无法使用。<p id="p10243143610134"><a name="p10243143610134"></a><a name="p10243143610134"></a>如果因为业务需求要将该数据盘扩容至2 TB以上并投入使用。则必须将MBR切换成GPT，期间会中断业务，并且更换分区形式时会清除数据盘原有数据，请在扩容前先对数据进行备份。</p>
</li></ul>
<a name="ul155151221015"></a><a name="ul155151221015"></a><ul id="ul155151221015"><li>当磁盘使用GPT分区形式时，容量最大支持18 EB（19327352832 GB）。由于EVS服务支持的最大数据盘容量为32 TB，因此使用GPT的数据盘最大可扩容至32 TB。</li></ul>
</div>
</td>
</tr>
<tr id="row878119815141"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p1378111851411"><a name="p1378111851411"></a><a name="p1378111851411"></a>将扩容部分的容量划分至已有的MBR分区内</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p67819814143"><a name="p67819814143"></a><a name="p67819814143"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section31113372194023">扩大已有MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p47818811414"><a name="p47818811414"></a><a name="p47818811414"></a><a href="#li069375552612">中断业务</a></p>
</td>
</tr>
<tr id="row278118171419"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p197816819146"><a name="p197816819146"></a><a name="p197816819146"></a>为扩容部分的云硬盘分配新的GPT分区</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p5781583147"><a name="p5781583147"></a><a name="p5781583147"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section15940163415487">新增GPT分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p778128121410"><a name="p778128121410"></a><a name="p778128121410"></a><a href="#li8782887145">不中断业务</a></p>
</td>
</tr>
<tr id="row1678119810147"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p97811082149"><a name="p97811082149"></a><a name="p97811082149"></a>将扩容部分的容量划分至已有的GPT分区内</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p17819819145"><a name="p17819819145"></a><a name="p17819819145"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section13346184710300">扩大已有GPT分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p197811284148"><a name="p197811284148"></a><a name="p197811284148"></a><a href="#li069375552612">中断业务</a></p>
</td>
</tr>
<tr id="row515711531178"><td class="cellrowborder" rowspan="2" valign="top" headers="mcps1.2.6.1.1 "><p id="p1115814536170"><a name="p1115814536170"></a><a name="p1115814536170"></a>SCSI数据盘</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p577312181820"><a name="p577312181820"></a><a name="p577312181820"></a>为扩容部分的云硬盘分配新的MBR分区</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p19158185371717"><a name="p19158185371717"></a><a name="p19158185371717"></a><a href="扩展SCSI数据盘的分区和文件系统（Linux）.md#section12265143819280">新增MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p20616228183"><a name="p20616228183"></a><a name="p20616228183"></a><a href="#li8782887145">不中断业务</a></p>
</td>
</tr>
<tr id="row544165520175"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p15771126185"><a name="p15771126185"></a><a name="p15771126185"></a>将扩容部分的容量划分至已有的MBR分区内</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p17442115501718"><a name="p17442115501718"></a><a name="p17442115501718"></a><a href="扩展SCSI数据盘的分区和文件系统（Linux）.md#section31113372194023">扩大已有MBR分区</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p19714223187"><a name="p19714223187"></a><a name="p19714223187"></a><a href="#li069375552612">中断业务</a></p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>系统盘：  
>-   <a name="li4674330102614"></a>不中断业务：新增分区时，不影响已有分区的使用，不会中断业务。  
>-   <a name="li132901912815"></a>依据Linux内核版本决定是否中断业务：若操作系统内核版本过低，需要**reboot**重启，扩展分区和文件系统才会生效，高版本内核则不需要重启。  
>数据盘：  
>-   <a name="li8782887145"></a>不中断业务：新增分区时，不影响已有分区的使用。推荐业务不中断的数据盘扩容场景使用。  
>-   <a name="li069375552612"></a>中断业务：扩大已有分区不会删除数据盘上的数据，但是需要通过**umount**命令先卸载已有分区，因此会影响线上业务运行。  

