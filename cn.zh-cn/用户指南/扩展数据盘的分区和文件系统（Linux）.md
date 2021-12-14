# 扩展数据盘的分区和文件系统（Linux）<a name="evs_01_0109"></a>

## 操作场景<a name="section4385650719406"></a>

通过云服务管理控制台扩容成功后，仅扩大了云硬盘的存储容量，因此需要参考本章节操作扩展分区和文件系统。

对于Linux操作系统而言，需要将扩容部分的容量划分至已有分区内，或者为扩容部分的云硬盘分配新的分区。

本文以“CentOS 7.4 64位”操作系统为例，提供MBR分区和GPT分区的操作指导。不同操作系统的操作可能不同，本文仅供参考，具体操作步骤和差异请参考对应操作系统的产品文档。

-   [扩大已有MBR分区或GPT分区](#section6227121018393)
-   [新增MBR分区](#section20200028194016)
-   [新增GPT分区](#section15940163415487)

>![](public_sys-resources/icon-notice.gif) **须知：** 
>扩容时请谨慎操作，误操作可能会导致数据丢失或者异常，建议扩容前对数据进行备份，可以使用CBR或者快照功能，CBR请参见[管理备份云硬盘](管理备份云硬盘.md)，快照功能请参见[创建快照（公测）](创建快照（公测）.md)。

## 前提条件<a name="section19088989195835"></a>

-   已通过管理控制台扩容云硬盘容量，并已挂载至云服务器，请参见[扩容“正在使用”状态的云硬盘容量](扩容-正在使用-状态的云硬盘容量.md)或者[扩容“可用”状态的云硬盘容量](扩容-可用-状态的云硬盘容量.md)。
-   已登录云服务器。
    -   弹性云服务器请参见[登录弹性云服务器](https://support.huaweicloud.com/qs-ecs/zh-cn_topic_0092494193.html)。
    -   裸金属服务器请参见[登录裸金属服务器](https://support.huaweicloud.com/qs-bms/bms_qs_0004.html)。

-   Linux操作系统内核版本不低于3.6.0。

    您可以使用**uname -a**命令查看Linux内核版本。内核版本低于3.6.0时，请参考[扩展磁盘分区和文件系统（Linux系统内核低于3.6.0）](https://support.huaweicloud.com/bestpractice-evs/evs_02_0025.html)。

-   扩容前的云硬盘已分区。

    针对没有分区的磁盘，解决方法请参见[Linux系统扩容数据盘时，如何扩展未分区磁盘文件系统](https://support.huaweicloud.com/evs_faq/evs_faq_0073.html)。


## 扩大已有MBR分区或GPT分区<a name="section6227121018393"></a>

数据盘“/dev/vdb”原有容量100GB，只有一个分区“/dev/vdb1”。将数据盘容量扩大至150GB，本示例将新增的50GB划分至已有的MBR分区或GPT分区内“/dev/vdb1”内。

1.  执行以下命令，安装growpart扩容工具。

    **yum install cloud-utils-growpart**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >可以用**growpart**命令检查当前系统是否已安装growpart扩容工具，若回显为工具使用介绍，则表示已安装，无需重复安装。

2.  <a name="li2047948185518"></a>执行以下命令，安装gdisk软件包。

    **yum install gdisk**

    系统提示

    ```
    Is this ok [y/d/N]: 
    ```

    输入“y”，按“Enter”，完成安装。

3.  执行以下命令，查看磁盘的分区信息。

    **fdisk** **-l**

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

4.  执行以下命令，查看数据盘分区“/dev/vdb1”的容量。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    devtmpfs       devtmpfs  509M     0  509M   0% /dev
    tmpfs          tmpfs     520M     0  520M   0% /dev/shm
    tmpfs          tmpfs     520M  7.1M  513M   2% /run
    tmpfs          tmpfs     520M     0  520M   0% /sys/fs/cgroup
    /dev/vda1      ext4       43G  2.3G   38G   6% /
    tmpfs          tmpfs     104M     0  104M   0% /run/user/0
    /dev/vdb1      ext4      106G   63M  101G   1% /mnt/sdc
    ```

5.  执行以下命令，指定数据盘待扩容的分区，通过growpart进行扩容。

    **growpart** _数据盘 分区编号_

    命令示例：

    **growpart /dev/vdb 1**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# growpart /dev/vdb 1
    CHANGED: partition=1 start=2048 old: size=209713152 end=209715200 new: size=314570719,end=314572767
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >若回显为
    >```
    >no tools available to resize disk with 'gpt'
    >FAILED: failed to get a resizer for id ''
    >```
    >请参考[2](#li2047948185518)安装gdisk软件包。

6.  根据磁盘的文件系统，选择不同方法扩展磁盘分区文件系统的大小。
    -   若磁盘文件系统为ext\*，请执行以下命令。

        **resize2fs** _磁盘分区_

        命令示例：

        **resize2fs /dev/vdb1**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# resize2fs /dev/vdb1
        resize2fs 1.42.9 (28-Dec-2013)
        Filesystem at /dev/vdb1 is mounted on /mnt/sdc; on-line resizing required
        old_desc_blocks = 13, new_desc_blocks = 19
        The filesystem on /dev/vdb1 is now 39321339 blocks long.
        ```

    -   若磁盘文件系统为xfs，请执行以下命令。

        **sudo** **xfs\_growfs** _磁盘分区_

        命令示例：

        **sudo** **xfs\_growfs /dev/vdb1**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# sudo xfs_growfs /dev/vdb1
        meta-data=/dev/vdb1              isize=512    agcount=4, agsize=6553472 blks
                 =                       sectsz=512   attr=2, projid32bit=1
                 =                       crc=1        finobt=0 spinodes=0
        data     =                       bsize=4096   blocks=26213888, imaxpct=25
                 =                       sunit=0      swidth=0 blks
        naming   =version 2              bsize=4096   ascii-ci=0 ftype=1
        log      =internal               bsize=4096   blocks=12799, version=2
                 =                       sectsz=512   sunit=0 blks, lazy-count=1
        realtime =none                   extsz=4096   blocks=0, rtextents=0
        data blocks changed from 26213888 to 39321339
        ```

7.  执行以下命令，查看扩容后数据盘分区“/dev/vdb1”的容量。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    devtmpfs       devtmpfs  509M     0  509M   0% /dev
    tmpfs          tmpfs     520M     0  520M   0% /dev/shm
    tmpfs          tmpfs     520M  7.1M  513M   2% /run
    tmpfs          tmpfs     520M     0  520M   0% /sys/fs/cgroup
    /dev/vda1      ext4       43G  2.3G   38G   6% /
    tmpfs          tmpfs     104M     0  104M   0% /run/user/0
    /dev/vdb1      ext4      159G   63M  151G   1% /mnt/sdc
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >重启后，挂载会失效。您可以修改“/etc/fstab”文件，将新建磁盘分区设置为开机自动挂载，请参见[设置开机自动挂载磁盘分区](#section1107170115310)。


## 新增MBR分区<a name="section20200028194016"></a>

数据盘“/dev/vdb”原有容量100GB，只有一个分区“/dev/vdb1”。将数据盘容量扩大至150GB，本示例为新增的50GB分配新的MBR分区“/dev/vdb2”。

1.  执行以下命令，查看磁盘的分区信息。

    **fdisk** **-l**

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

2.  执行以下命令，进入fdisk分区工具。

    **fdisk** _磁盘_

    命令示例：

    **fdisk** **/dev/vdb**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# fdisk /dev/vdb
    Welcome to fdisk (util-linux 2.23.2).
    
    Changes will remain in memory only, until you decide to write them.
    Be careful before using the write command.
    
    
    Command (m for help): 
    ```

3.  输入“n”，按“Enter”，开始新建分区。

    回显类似如下信息：

    ```
    Command (m for help): n
    Partition type:
       p   primary (1 primary, 0 extended, 3 free)
       e   extended
    Select (default p):
    ```

    表示磁盘有两种分区类型：

    -   “p“表示主分区。
    -   “e“表示扩展分区。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >磁盘使用MBR分区形式，最多可以创建4个主分区，或者3个主分区加1个扩展分区，扩展分区不可以直接使用，需要划分成若干个逻辑分区才可以使用。
    >磁盘使用GPT分区形式时，没有主分区、扩展分区以及逻辑分区之分。

4.  以创建一个主分区为例，输入“p”，按“Enter”。

    回显类似如下信息：

    ```
    Select (default p): p
    Partition number (2-4, default 2):
    ```

    “Partition number“表示主分区编号，可以选择2-4，由于1已被使用，此处从2开始。

5.  以分区编号选择“2”为例，输入分区编号“2”，按“Enter”。

    回显类似如下信息：

    ```
    Partition number (2-4, default 2): 2
    First sector (209715200-314572799, default 209715200):
    ```

    “First sector”表示起始磁柱值，可以选择209715200-314572799，默认为209715200。

6.  输入新分区的起始磁柱值，以使用默认起始磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    First sector (209715200-314572799, default 209715200):
    Using default value 209715200
    Last sector, +sectors or +size{K,M,G} (209715200-314572799, default 314572799):
    ```

    “Last sector”表示截止磁柱值，可以选择209715200-314572799，默认为314572799。

7.  输入新分区的截止磁柱值，以使用默认截止磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    Last sector, +sectors or +size{K,M,G} (209715200-314572799, default 314572799):
    Using default value 314572799
    Partition 2 of type Linux and of size 50 GiB is set
    
    Command (m for help): 
    ```

8.  输入“p”，按“Enter”，查看新建分区。

    回显类似如下信息：

    ```
    Command (m for help): p
    
    Disk /dev/vdb: 161.1 GB, 161061273600 bytes, 314572800 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x38717fc1
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vdb1            2048   209715199   104856576   83  Linux
    /dev/vdb2       209715200   314572799    52428800   83  Linux
    
    Command (m for help): 
    ```

9.  输入“w”，按“Enter”，将分区结果写入分区表中。

    回显类似如下信息：

    ```
    Command (m for help): w
    The partition table has been altered!
    
    Calling ioctl() to re-read partition table.
    
    WARNING: Re-reading the partition table failed with error 16: Device or resource busy.
    The kernel still uses the old table. The new table will be used at
    the next reboot or after you run partprobe(8) or kpartx(8)
    Syncing disks.
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果之前分区操作有误，请输入“q”，则会退出fdisk分区工具，之前的分区结果将不会被保留。

10. 执行以下命令，将新的分区表变更同步至操作系统。

    **partprobe**

11. 执行以下命令，为新建分区设置文件系统。

    **mkfs** **-t** _文件系统_ _磁盘分区_

    -   ext\*文件系统命令示例：

        **mkfs** **-t** **ext4** **/dev/vdb2**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# mkfs -t ext4 /dev/vdb2
        mke2fs 1.42.9 (28-Dec-2013)
        Filesystem label=
        OS type: Linux
        Block size=4096 (log=2)
        Fragment size=4096 (log=2)
        Stride=0 blocks, Stripe width=0 blocks
        3276800 inodes, 13107200 blocks
        655360 blocks (5.00%) reserved for the super user
        First data block=0
        Maximum filesystem blocks=2162163712
        400 block groups
        32768 blocks per group, 32768 fragments per group
        8192 inodes per group
        Superblock backups stored on blocks:
                32768, 98304, 163840, 229376, 294912, 819200, 884736, 1605632, 2654208,
                4096000, 7962624, 11239424
        
        Allocating group tables: done
        Writing inode tables: done
        Creating journal (32768 blocks): done
        Writing superblocks and filesystem accounting information: done
        ```

    -   xfs文件系统命令示例：

        **mkfs** **-t** **xfs** **/dev/vdb2**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# mkfs -t xfs /dev/vdb2 
        meta-data=/dev/vdb2              isize=512     agcount=4, agsize=3276800 blks
                 =                       sectsz=512    attr=2, projid32bit=1
                 =                       crc=1         finobt=0, sparse=0
        data     =                       bsize=4096    blocks=13107200, imaxpct=25
                 =                       sunit=0       swidth=0 blks
        naming   =version2               bsize=4096    ascii-ci=0 ftype=1
        log      =internal log           bsize=4096    blocks=6400, version=2
                 =                       sectsz=512    sunit=0 blks, lazy-count=1
        realtime =none                   extsz=4096    blocks=0, rtextents=0
        ```

    格式化需要等待一段时间，请观察系统运行状态，若回显中进程提示为done，则表示格式化完成。

12. （可选）执行以下命令，新建挂载目录。

    若需要挂载至新建目录下，执行该操作。

    **mkdir** _挂载目录_

    以新建挂载目录“/mnt/test”为例：

    **mkdir** **/mnt/test**

13. 执行以下命令，挂载新建分区。

    **mount** _磁盘分区_ _挂载目录_

    以挂载新建分区“/dev/vdb2”至“/mn/test”为例：

    **mount** **/dev/vdb2** **/mnt/test**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。

14. 执行以下命令，查看挂载结果。

    **df** **-TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  1.9G   39G   5% /
    devtmpfs       devtmpfs  2.0G     0  2.0G   0% /dev
    tmpfs          tmpfs     2.0G     0  2.0G   0% /dev/shm
    tmpfs          tmpfs     2.0G  9.1M  2.0G   1% /run
    tmpfs          tmpfs     2.0G     0  2.0G   0% /sys/fs/cgroup
    tmpfs          tmpfs     398M     0  398M   0% /run/user/0
    /dev/vdb1      ext4      106G   63M  101G   1% /mnt/sdc
    /dev/vdb2      ext4       53G   55M   50G   1% /mnt/test
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >云服务器重启后，挂载会失效。您可以修改“/etc/fstab”文件，将新建磁盘分区设置为开机自动挂载，请参见[设置开机自动挂载磁盘分区](#section1107170115310)。


## 新增GPT分区<a name="section15940163415487"></a>

数据盘“/dev/vdb”原有容量100GB，只有一个分区“/dev/vdb1”。将数据盘容量扩大至150GB，本示例为新增的50GB分配新的GPT分区“/dev/vdb2”。

1.  执行以下命令，查看磁盘的分区信息。

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

2.  <a name="li131751636184912"></a>执行以下命令，进入parted分区工具。

    **parted**  磁盘

    命令示例：

    **parted** **/dev/vdb**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# parted /dev/vdb
    GNU Parted 3.1
    Using /dev/vdb
    Welcome to GNU Parted! Type 'help' to view a list of commands.
    (parted) 
    ```

3.  输入“unit s”，按“Enter”，设置磁盘的计量单位为磁柱。
4.  <a name="li317653664918"></a>输入“p”，按“Enter”，查看当前磁盘分区情况。

    回显类似如下信息：

    ```
    (parted) unit s
    (parted) p
    Error: The backup GPT table is not at the end of the disk, as it should be.  This might mean that another operating system believes the
    disk is smaller.  Fix, by moving the backup to the end (and removing the old backup)?
    Fix/Ignore/Cancel? Fix
    Warning: Not all of the space available to /dev/vdb appears to be used, you can fix the GPT to use all of the space (an extra 104857600
    blocks) or continue with the current setting?
    Fix/Ignore? Fix
    Model: Virtio Block Device (virtblk)
    Disk /dev/vdb: 314572800s
    Sector size (logical/physical): 512B/512B
    Partition Table: gpt
    Disk Flags:
    
    Number  Start  End         Size        File system  Name  Flags
     1      2048s  209713151s  209711104s  ext4         test
    
    (parted)
    ```

    记录已有分区的截止磁柱值（End），本示例中已有分区“/dev/vdb1”的截止磁柱值为209713151s。

    -   若系统出现以下Error，请输入“Fix”。

        ```
        Error: The backup GPT table is not at the end of the disk, as it should be.  This might mean that another operating system believes the
        disk is smaller.  Fix, by moving the backup to the end (and removing the old backup)?
        ```

        GPT分区表信息存储在磁盘开头，为了减少分区表损坏的风险，同时在磁盘末尾会备份一份。当磁盘容量扩大后，末尾位置也会随之变化，因此需要根据系统提示输入“Fix”，将分区表信息的备份文件挪到新的磁盘末尾位置。

    -   若系统出现以下Waring，请输入“Fix”。

        ```
        Warning: Not all of the space available to /dev/vdb appears to be used, you can fix the GPT to use all of the space (an extra 104857600
        blocks) or continue with the current setting?
        Fix/Ignore? Fix
        ```

        根据系统提示输入“Fix”，系统会自动将磁盘扩容部分的容量设置为GPT。

5.  以为新增容量分配一整个分区为例，执行以下命令，按“Enter”。

    **mkpart** _磁盘分区名称 起始磁柱值_ _截止磁柱__值_

    命令示例：

    **mkpart** **data** **209713152s** **100%**

    由于[4](#li317653664918)中，已有分区“dev/vdb1”的截止磁柱值为“209713151s”，因此对于新增分区“dev/vdb2”，起始磁柱值设置为“209713152s”，截止磁柱值设置为“100%”。此处仅供参考，您可以根据业务需要自行规划磁盘分区数量及容量。

    回显类似如下信息：

    ```
    (parted) mkpart data 209713152s 100%
    (parted) 
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >获取最大截止磁柱值的方法如下：
    >-   参考[2](#li131751636184912)\~[4](#li317653664918)，查询磁盘的最大截止磁柱值。
    >-   可以输入**-1s**或者**100%**，即默认为磁盘的最大截止磁柱值。

6.  输入“p”，按“Enter”，查看新建分区。

    回显类似如下信息：

    ```
    (parted) p
    Model: Virtio Block Device (virtblk)
    Disk /dev/vdb: 314572800s
    Sector size (logical/physical): 512B/512B
    Partition Table: gpt
    Disk Flags:
    
    Number  Start       End         Size        File system  Name  Flags
     1      2048s       209713151s  209711104s  ext4         test
     2      209713152s  314570751s  104857600s               data
    
    (parted) 
    ```

7.  输入“q”，按“Enter”，退出parted分区工具。

    回显类似如下信息：

    ```
    (parted) q
    Information: You may need to update /etc/fstab.
    ```

    “/etc/fstab”文件控制磁盘开机自动挂载，请先参考以下步骤为磁盘分区设置文件系统和挂载目录后，再根据文档指导更新“/etc/fstab”文件。

8.  执行以下命令，为新建分区设置文件系统。

    **mkfs** **-t** _文件系统_ _磁盘分区_

    -   ext\*文件系统命令示例：

        **mkfs** **-t** **ext4** **/dev/vdb2**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# mkfs -t ext4 /dev/vdb2
        mke2fs 1.42.9 (28-Dec-2013)
        Filesystem label=
        OS type: Linux
        Block size=4096 (log=2)
        Fragment size=4096 (log=2)
        Stride=0 blocks, Stripe width=0 blocks
        3276800 inodes, 13107200 blocks
        655360 blocks (5.00%) reserved for the super user
        First data block=0
        Maximum filesystem blocks=2162163712
        400 block groups
        32768 blocks per group, 32768 fragments per group
        8192 inodes per group
        Superblock backups stored on blocks:
                32768, 98304, 163840, 229376, 294912, 819200, 884736, 1605632, 2654208,
                4096000, 7962624, 11239424
        
        Allocating group tables: done
        Writing inode tables: done
        Creating journal (32768 blocks): done
        Writing superblocks and filesystem accounting information: done
        ```

    -   xfs文件系统命令示例：

        **mkfs** **-t** **xfs** **/dev/vdb2**

        回显类似如下信息：

        ```
        [root@ecs-test-0001 ~]# mkfs -t xfs /dev/vdb2 
        meta-data=/dev/vdb2              isize=512     agcount=4, agsize=3276800 blks
                 =                       sectsz=512    attr=2, projid32bit=1
                 =                       crc=1         finobt=0, sparse=0
        data     =                       bsize=4096    blocks=13107200, imaxpct=25
                 =                       sunit=0       swidth=0 blks
        naming   =version2               bsize=4096    ascii-ci=0 ftype=1
        log      =internal log           bsize=4096    blocks=6400, version=2
                 =                       sectsz=512    sunit=0 blks, lazy-count=1
        realtime =none                   extsz=4096    blocks=0, rtextents=0
        ```

    格式化需要等待一段时间，请观察系统运行状态，若回显中进程提示为done，则表示格式化完成。

9.  （可选）执行以下命令，新建挂载目录。

    若需要挂载至新建目录下，执行该操作。

    **mkdir** _挂载目录_

    以新建挂载目录“/mnt/test”为例：

    **mkdir** **/mnt/test**

10. 执行以下命令，挂载新建分区。

    **mount** _磁盘分区_ _挂载目录_

    以挂载新建分区“/dev/vdb2”至“/mn/test”为例：

    **mount** **/dev/vdb2** **/mnt/test**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。

11. 执行以下命令，查看挂载结果。

    **df** **-TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  1.9G   39G   5% /
    devtmpfs       devtmpfs  2.0G     0  2.0G   0% /dev
    tmpfs          tmpfs     2.0G     0  2.0G   0% /dev/shm
    tmpfs          tmpfs     2.0G  9.1M  2.0G   1% /run
    tmpfs          tmpfs     2.0G     0  2.0G   0% /sys/fs/cgroup
    tmpfs          tmpfs     398M     0  398M   0% /run/user/0
    /dev/vdb1      ext4      106G   63M  101G   1% /mnt/sdc
    /dev/vdb2      ext4       53G   55M   50G   1% /mnt/test
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >云服务器重启后，挂载会失效。您可以修改“/etc/fstab”文件，将新建磁盘分区设置为开机自动挂载，请参见[设置开机自动挂载磁盘分区](#section1107170115310)。


## 设置开机自动挂载磁盘分区<a name="section1107170115310"></a>

您可以通过配置fstab文件，设置云服务器系统启动时自动挂载磁盘分区。

本文介绍如何在fstab文件中使用UUID来设置自动挂载磁盘分区。不建议采用在“/etc/fstab”直接指定设备名（比如/dev/vdb1）的方法，因为云中设备的顺序编码在关闭或者开启云服务器过程中可能发生改变，例如/dev/vdb1可能会变成/dev/vdb2，可能会导致云服务器重启后不能正常运行。

>![](public_sys-resources/icon-note.gif) **说明：** 
>UUID（universally unique identifier）是Linux系统为磁盘分区提供的唯一的标识字符串。

1.  <a name="zh-cn_topic_0044524669_li840964143216"></a>执行如下命令，查询磁盘分区的UUID。

    **blkid** _磁盘分区_

    以查询磁盘分区“/dev/vdb1“的UUID为例：

    **blkid /dev/vdb1**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# blkid /dev/vdb1
    /dev/vdb1: UUID="0b3040e2-1367-4abb-841d-ddb0b92693df" TYPE="ext4"
    ```

    表示“/dev/vdb1“的UUID。

2.  执行以下命令，使用VI编辑器打开“fstab”文件。

    **vi /etc/fstab**

3.  按“i”，进入编辑模式。
4.  将光标移至文件末尾，按“Enter”，添加如下内容。

    ```
    UUID=0b3040e2-1367-4abb-841d-ddb0b92693df /mnt/sdc                ext4    defaults        0 2
    ```

    以内容上仅为示例，具体请以实际情况为准，参数说明如下：

    -   第一列为UUID，此处填写[1](#zh-cn_topic_0044524669_li840964143216)中查询到的磁盘分区的UUID。
    -   第二列为磁盘分区的挂载目录，可以通过**df -TH**命令查询。
    -   第三列为磁盘分区的文件系统格式， 可以通过**df -TH**命令查询。
    -   第四列为磁盘分区的挂载选项，此处通常设置为defaults即可。
    -   第五列为Linux dump备份选项。
        -   0表示不使用Linux dump备份。现在通常不使用dump备份，此处设置为0即可。
        -   1表示使用Linux dump备份。

    -   第六列为fsck选项，即开机时是否使用fsck检查磁盘。
        -   0表示不检验。
        -   挂载点为（/）根目录的分区，此处必须填写1。

            根分区设置为1，其他分区只能从2开始，系统会按照数字从小到大依次检查下去。


5.  按“ESC”后，输入“:wq”，按“Enter”。

    保存设置并退出编辑器。

6.  执行以下步骤，验证自动挂载功能。
    1.  执行如下命令，卸载已挂载的分区。

        **umount** _磁盘分区_

        命令示例：

        **umount /dev/vdb1**

    2.  执行如下命令，将“/etc/fstab”文件所有内容重新加载。

        **mount -a**

    3.  执行如下命令，查询文件系统挂载信息。

        **mount** **|** **grep** _挂载目录_

        命令示例：

        **mount** **|** **grep** **/mnt/sdc**

        回显类似如下信息，说明自动挂载功能生效：

        ```
        root@ecs-test-0001 ~]# mount | grep /mnt/sdc
        /dev/vdb1 on /mnt/sdc type ext4 (rw,relatime,data=ordered)
        ```



