# 分区和文件系统扩展前准备（Linux）<a name="evs_01_0035"></a>

扩展磁盘分区和文件系统前，请先检查磁盘的分区形式和文件系统，并根据磁盘的分区形式选择对应的操作指导。

1.  检查磁盘分区形式，请参见：
    -   [方法一：使用fdisk命令查看分区形式和文件系统](#section45741613172812)
    -   [方法二：使用parted命令查看分区形式和文件系统](#section7627683297)

2.  扩展磁盘分区和文件系统，请参见[表1](#table454986114415)。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >以下操作指导仅适用于内核版本不低于3.6.0的Linux操作系统。
    >您可以使用**uname -a**命令查看Linux内核版本。内核版本低于3.6.0时，请参考[扩展磁盘分区和文件系统（Linux系统内核低于3.6.0）](https://support.huaweicloud.com/bestpractice-evs/evs_02_0025.html)。

    **表 1**  分区和文件系统扩展场景说明

    <a name="table454986114415"></a>
    <table><thead align="left"><tr id="row75491662440"><th class="cellrowborder" valign="top" width="10.280000000000001%" id="mcps1.2.4.1.1"><p id="p5549136194411"><a name="p5549136194411"></a><a name="p5549136194411"></a>磁盘</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.29%" id="mcps1.2.4.1.2"><p id="p85491618442"><a name="p85491618442"></a><a name="p85491618442"></a>场景</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.43%" id="mcps1.2.4.1.3"><p id="p8549116194411"><a name="p8549116194411"></a><a name="p8549116194411"></a>方法</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1094814319216"><td class="cellrowborder" rowspan="2" valign="top" width="10.280000000000001%" headers="mcps1.2.4.1.1 "><p id="p1794819310212"><a name="p1794819310212"></a><a name="p1794819310212"></a>系统盘</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p354986104413"><a name="p354986104413"></a><a name="p354986104413"></a>将扩容部分的容量划分至已有的MBR分区内</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.43%" headers="mcps1.2.4.1.3 "><p id="p10471396558"><a name="p10471396558"></a><a name="p10471396558"></a><a href="扩展系统盘的分区和文件系统（Linux）.md#section9613733145218">扩大已有MBR分区</a></p>
    </td>
    </tr>
    <tr id="row12549569442"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p155491667446"><a name="p155491667446"></a><a name="p155491667446"></a>为扩容部分的云硬盘分配新的MBR分区</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p155498615442"><a name="p155498615442"></a><a name="p155498615442"></a><a href="扩展系统盘的分区和文件系统（Linux）.md#section9194153012119">新增MBR分区</a></p>
    </td>
    </tr>
    <tr id="row1717621415212"><td class="cellrowborder" rowspan="4" valign="top" width="10.280000000000001%" headers="mcps1.2.4.1.1 "><p id="p15177131410213"><a name="p15177131410213"></a><a name="p15177131410213"></a>数据盘</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p95495611448"><a name="p95495611448"></a><a name="p95495611448"></a>将扩容部分的容量划分至已有的MBR分区内</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.43%" headers="mcps1.2.4.1.3 "><p id="p95491461443"><a name="p95491461443"></a><a name="p95491461443"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section6227121018393">扩大已有MBR分区或GPT分区</a></p>
    </td>
    </tr>
    <tr id="row35498614447"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1854917664420"><a name="p1854917664420"></a><a name="p1854917664420"></a>为扩容部分的云硬盘分配新的MBR分区</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p1754915610449"><a name="p1754915610449"></a><a name="p1754915610449"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section20200028194016">新增MBR分区</a></p>
    </td>
    </tr>
    <tr id="row1154915694418"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p12549369449"><a name="p12549369449"></a><a name="p12549369449"></a>将扩容部分的容量划分至已有的GPT分区内</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p0549196104417"><a name="p0549196104417"></a><a name="p0549196104417"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section6227121018393">扩大已有MBR分区或GPT分区</a></p>
    </td>
    </tr>
    <tr id="row105492068441"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1854996154416"><a name="p1854996154416"></a><a name="p1854996154416"></a>为扩容部分的云硬盘分配新的GPT分区</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p185491664412"><a name="p185491664412"></a><a name="p185491664412"></a><a href="扩展数据盘的分区和文件系统（Linux）.md#section15940163415487">新增GPT分区</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >MBR分区支持的磁盘最大容量为2 TB，超过2 TB的部分无法使用。
    >如果当前磁盘采用MBR分区形式，并且需要将该磁盘扩容至2 TB以上投入使用。则必须将磁盘分区形式由MBR切换成GPT，期间会中断业务，并且更换磁盘分区形式时会清除磁盘的原有数据，请在扩容前先对数据进行备份。


## 方法一：使用fdisk命令查看分区形式和文件系统<a name="section45741613172812"></a>

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
    >如果执行了**lsblk**，发现磁盘“/dev/vdb”没有分区，针对这种没有分区的磁盘，扩容后的容量可能无法正常使用，解决方法请参见[Linux系统扩容数据盘时，如何扩展未分区磁盘文件系统](https://support.huaweicloud.com/evs_faq/evs_faq_0073.html)。

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

    -   若回显中没有列出所有的磁盘分区，和[1](#li4640174163019)中的信息不符合。可能原因是：磁盘已有分区为GPT，并且扩容后存在未分配分区的空间，此时使用**fdisk -l**无法查看所有分区的信息，请参考[方法二：使用parted命令查看分区形式和文件系统](#section7627683297)重新确认磁盘分区形式和文件系统。
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


## 方法二：使用parted命令查看分区形式和文件系统<a name="section7627683297"></a>

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
    >如果执行了**lsblk**，发现磁盘“/dev/vdb”没有分区，针对这种没有分区的磁盘，扩容后的容量可能无法正常使用，解决方法请参见[Linux系统扩容数据盘时，如何扩展未分区磁盘文件系统](https://support.huaweicloud.com/evs_faq/evs_faq_0073.html)。

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

