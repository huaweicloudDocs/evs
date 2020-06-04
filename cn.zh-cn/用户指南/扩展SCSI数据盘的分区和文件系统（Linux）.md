# 扩展SCSI数据盘的分区和文件系统（Linux）<a name="evs_01_0018"></a>

## 操作场景<a name="section4385650719406"></a>

通过云服务管理控制台扩容成功后，仅扩大了云硬盘的存储容量，因此需要参考本章节操作扩展分区和文件系统。

对于linux操作系统而言，需要将扩容部分的容量划分至已有分区内，或者为扩容部分的云硬盘分配新的分区。

本文以“CentOS 7.4 64位”操作系统为例，提供针对SCSI数据盘的MBR分区的操作指导。不同操作系统的操作可能不同，本文仅供参考，具体操作步骤和差异请参考对应操作系统的产品文档。

-   [新增MBR分区](#section12265143819280)
-   [扩大已有MBR分区](#section31113372194023)

>![](public_sys-resources/icon-notice.gif) **须知：**   
>扩容时请谨慎操作，误操作可能会导致数据丢失或者异常，建议扩容前对数据进行备份，可以使用CBR或者快照功能，CBR请参见[管理备份云硬盘](管理备份云硬盘.md)，快照功能请参见[创建快照（公测）](创建快照（公测）.md)。  

## 前提条件<a name="section19088989195835"></a>

-   已通过管理控制台扩容云硬盘容量，并已挂载至云服务器，请参见[扩容“正在使用”状态的云硬盘容量](扩容-正在使用-状态的云硬盘容量.md)或者[扩容“可用”状态的云硬盘容量](扩容-可用-状态的云硬盘容量.md)。
-   已登录云服务器。
    -   弹性云服务器请参见[登录弹性云服务器](https://support.huaweicloud.com/qs-ecs/zh-cn_topic_0092494193.html)。
    -   裸金属服务器请参见[登录裸金属服务器](https://support.huaweicloud.com/qs-bms/bms_qs_0004.html)。


## 新增MBR分区<a name="section12265143819280"></a>

数据盘“/dev/sda”原有容量50GB，只有一个分区“/dev/sda1”。将数据盘容量扩大至100GB，本示例为新增的50GB分配新的MBR分区“/dev/sda2”。

1.  执行以下命令，查看磁盘的分区信息。

    **fdisk -l**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# fdisk -l
    
    Disk /dev/vda: 42.9 GB, 42949672960 bytes, 83886080 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000bcb4e
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    
    Disk /dev/sda: 107.4 GB, 107374182400 bytes, 209715200 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x915ffe6a
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1            2048   104857599    52427776   83  Linux
    ```

    查看回显中SCSI数据盘“/dev/sda”的容量，扩容的容量是否已经包含在容量总和中。

    -   若扩容的容量未在数据盘容量总和中，请执行[2](#li1311112192367)刷新系统内容量。
    -   若扩容的容量已在数据盘容量总和中，请执行[3](#li14771329195025)。

2.  <a name="li1311112192367"></a>（可选）执行以下步骤，刷新系统内SCSI数据盘的容量。
    1.  执行以下命令，刷新云服务器内SCSI数据盘的容量。

        **echo 1 \> /sys/class/scsi\_device/**_%d:%d:%d:%d_**/device/rescan &**

        其中“%d:%d:%d:%d”为“/sys/class/scsi\_device/”路径下的文件夹，执行**ll /sys/class/scsi\_device/**命令获取。

        回显类似如下信息，“2:0:0:0”即为待获取的文件夹。

        ```
        cs-xen-02:/sys/class/scsi_device # ll /sys/class/scsi_device/
        total 0
        lrwxrwxrwx 1 root root 0 Sep 26 11:37 2:0:0:0 -> ../../devices/xen/vscsi-2064/host2/target2:0:0/2:0:0:0/scsi_device/2:0:0:0
        ```

        命令示例：

        **echo 1 \> /sys/class/scsi\_device/2:0:0:0/device/rescan &**

    2.  刷新完成后，执行以下命令，再次查看磁盘分区信息。

        **fdisk -l**

        若扩容的容量已在数据盘容量总和中，请执行[3](#li14771329195025)。

3.  <a name="li14771329195025"></a>执行以下命令，进入fdisk分区工具。

    **fdisk** _磁盘_

    命令示例：

    **fdisk /dev/sda**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# fdisk /dev/sda
    Welcome to fdisk (util-linux 2.23.2).
    
    Changes will remain in memory only, until you decide to write them.
    Be careful before using the write command.
    
    
    Command (m for help):
    ```

4.  输入“n”，按“Enter”，开始新建分区。

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

5.  以创建一个主分区为例，输入“p”，按“Enter”。

    回显类似如下信息：

    ```
    Select (default p): p
    Partition number (2-4, default 2):
    ```

    “Partition number“表示主分区编号，可以选择2-4，由于1已被使用，此处从2开始。

6.  以分区编号选择“2”为例，输入分区编号“2”，按“Enter”。

    回显类似如下信息：

    ```
    Partition number (2-4, default 2): 2
    First sector (104857600-209715199, default 104857600):
    ```

    “First sector”表示起始磁柱值，可以选择104857600-209715199，默认为104857600。

7.  输入新分区的起始磁柱值，以使用默认起始磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    First sector (104857600-209715199, default 104857600):
    Using default value 104857600
    Last sector, +sectors or +size{K,M,G} (104857600-209715199, default 209715199):
    ```

    “Last sector”表示截止磁柱值，可以选择104857600-209715199，默认为209715199。

8.  输入新分区的截止磁柱值，以使用默认截止磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    Last sector, +sectors or +size{K,M,G} (104857600-209715199, default 209715199):
    Using default value 209715199
    Partition 2 of type Linux and of size 50 GiB is set
    
    Command (m for help):
    ```

9.  输入“p”，按“Enter”，查看新建分区。

    回显类似如下信息：

    ```
    Command (m for help): p
    
    Disk /dev/sda: 107.4 GB, 107374182400 bytes, 209715200 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x915ffe6a
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1            2048   104857599    52427776   83  Linux
    /dev/sda2       104857600   209715199    52428800   83  Linux
    
    Command (m for help):
    ```

10. 输入“w”，按“Enter”，将分区结果写入分区表中。

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

11. 执行以下命令，将新的分区表变更同步至操作系统。

    **partprobe**

12. 执行以下命令，为新建分区设置文件系统。

    **mkfs -t** _文件系统_ _磁盘分区_

    -   ext\*文件系统命令示例：

        **mkfs -t ext4 /dev/sda2**

        回显类似如下信息：

        ```
        [root@ecs-scsi ~]# mkfs -t ext4 /dev/sda2
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

    -   xfs文件系统命名示例：

        **mkfs -t xfs /dev/sda2**

        回显类似如下信息：

        ```
        [root@ecs-scsi ~]# mkfs -t xfs /dev/sda2
        meta-data=/dev/sda2              isize=512     agcount=4, agsize=3276800 blks
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

13. （可选）执行以下命令，新建挂载目录。

    若需要挂载至新建目录下，执行该操作。

    **mkdir** _挂载目录_

    以新建挂载目录“/mnt/test”为例：

    **mkdir** **/mnt/test**

14. 执行以下命令，挂载新建分区。

    **mount** _磁盘分区_ _挂载目录_

    以挂载新建分区“/dev/sda2”至“/mn/test”为例：

    **mount /dev/sda2 /mnt/test**

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。  

15. 执行以下命令，查看挂载结果。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  2.0G   39G   5% /
    devtmpfs       devtmpfs  509M     0  509M   0% /dev
    tmpfs          tmpfs     520M     0  520M   0% /dev/shm
    tmpfs          tmpfs     520M  7.2M  513M   2% /run
    tmpfs          tmpfs     520M     0  520M   0% /sys/fs/cgroup
    tmpfs          tmpfs     104M     0  104M   0% /run/user/0
    /dev/sda1      ext4       53G   55M   50G   1% /mnt/sdc
    /dev/sda2      ext4       53G   55M   50G   1% /mnt/test
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >云服务器重启后，挂载会失效。您可以修改“/etc/fstab”文件，将新建磁盘分区设置为开机自动挂载，请参见[设置开机自动挂载磁盘分区](#section1107170115310)。  


## 扩大已有MBR分区<a name="section31113372194023"></a>

>![](public_sys-resources/icon-notice.gif) **须知：**   
>扩大已有分区不会删除数据盘上的数据，但是需要通过umount命令先卸载已有分区，因此会影响线上业务运行。  

SCSI数据盘“/dev/sda”原有容量100GB，有两个分区“/dev/sda1 ”和“/dev/sda2”。将数据盘容量扩大至150GB，本示例将新增的50GB划分至已有的MBR分区“/dev/sda2”内。

扩容后的新增存储空间是添加在磁盘末尾的，对具有多个分区的的磁盘扩容时，只支持将新增容量划分至排在末尾的分区。

1.  <a name="li6396237219479"></a>执行以下命令，查看磁盘的分区信息。

    **fdisk -l**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# fdisk -l
    
    Disk /dev/vda: 42.9 GB, 42949672960 bytes, 83886080 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000bcb4e
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    
    Disk /dev/sda: 161.1 GB, 161061273600 bytes, 314572800 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x915ffe6a
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1            2048   104857599    52427776   83  Linux
    /dev/sda2       104857600   209715199    52428800   83  Linux
    ```

    记录待扩大分区的起始磁柱值（Start）和截止磁柱值（End），本示例中待扩大分区“/dev/sda2”的起始磁柱值为104857600，截止磁柱值为209715199。

    查看回显中SCSI数据盘“/dev/sda”的容量，扩容的容量是否已经包含在容量总和中。

    -   若扩容的容量未在数据盘容量总和中，请执行[2](#li11239195417383)刷新系统内容量。
    -   若扩容的容量已在数据盘容量总和中，请记录待扩大分区的起始和截止磁柱值，这些值在后续重新创建分区时需要使用，记录完成后执行[3](#li3879043619479)。

2.  <a name="li11239195417383"></a>（可选）执行以下步骤，刷新系统内SCSI数据盘的容量。
    1.  执行以下命令，刷新云服务器内SCSI数据盘的容量。

        **echo 1 \> /sys/class/scsi\_device/**_%d:%d:%d:%d_**/device/rescan &**

        其中“%d:%d:%d:%d”为“/sys/class/scsi\_device/”路径下的文件夹，执行**ll /sys/class/scsi\_device/**命令获取。

        回显类似如下信息，“2:0:0:0”即为待获取的文件夹。

        ```
        cs-xen-02:/sys/class/scsi_device # ll /sys/class/scsi_device/
        total 0
        lrwxrwxrwx 1 root root 0 Sep 26 11:37 2:0:0:0 -> ../../devices/xen/vscsi-2064/host2/target2:0:0/2:0:0:0/scsi_device/2:0:0:0
        ```

        命令示例：

        **echo 1 \> /sys/class/scsi\_device/2:0:0:0/device/rescan &**

    2.  刷新完成后，执行以下命令，再次查看磁盘分区信息。

        **fdisk -l**

        若扩容的容量已在数据盘容量总和中，请记录待扩大分区的起始和截止磁柱值，这些值在后续重新创建分区时需要使用，记录完成后执行[3](#li3879043619479)。

3.  <a name="li3879043619479"></a>执行如下命令，卸载磁盘分区。

    **umount** _磁盘分区_

    命令示例：

    **umount /dev/sda2**

4.  执行以下命令，进入fdisk分区工具。

    **fdisk** _磁盘_

    命令示例：

    **fdisk /dev/sda**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# fdisk /dev/sda
    Welcome to fdisk (util-linux 2.23.2).
    
    Changes will remain in memory only, until you decide to write them.
    Be careful before using the write command.
    
    
    Command (m for help):
    ```

5.  执行以下步骤，删除待扩大的分区。
    1.  输入“d”，按“Enter”，删除磁盘分区。

        回显类似如下信息：

        ```
        Command (m for help): d
        Partition number (1,2, default 2):
        ```

    2.  输入分区编号，此处以分区编号选择“2”为例，按“Enter”，删除磁盘分区。

        回显类似如下信息：

        ```
        Partition number (1,2, default 2): 2
        Partition 2 is deleted
        
        Command (m for help): 
        ```

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >删除分区后，请参考以下操作步骤扩大原有分区，则不会导致数据盘内数据的丢失。  


6.  输入“n”，按“Enter”，开始新建分区。

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

7.  此处分区类型需要与原分区保持一致，以原分区类型是主要分区为例，输入“p”，按“Enter”，开始重新创建一个主分区。

    回显类似如下信息：

    ```
    Select (default p): p
    Partition number (2-4, default 2):
    ```

    “Partition number“表示主分区编号。

8.  此处分区编号需要与原分区保持一致，以原分区编号是“2”为例，输入分区编号“2”，按“Enter”。

    回显类似如下信息：

    ```
    Partition number (2-4, default 2): 2
    First sector (104857600-314572799, default 104857600):
    ```

    “First sector“表示起始磁柱值。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >以下操作会导致数据丢失：  
    >-   选择的起始磁柱值与原分区的不一致。  
    >-   选择的截止磁柱值小于原分区的值。  

9.  此处必须与原分区保持一致，输入[1](#li6396237219479)或者[2](#li11239195417383)记录的起始磁柱值104857600，此处该值也为默认值，按“Enter”。

    回显类似如下信息：

    ```
    First sector (104857600-314572799, default 104857600):
    Using default value 104857600
    Last sector, +sectors or +size{K,M,G} (104857600-314572799, default 314572799):
    ```

    “Last sector“表示截止磁柱值。

10. 此处截止磁柱值应大于等于[1](#li6396237219479)或者[2](#li11239195417383)中记录的截止磁柱值209715199，以选择默认截止磁柱值314572799为例，按“Enter”。

    回显类似如下信息：

    ```
    Last sector, +sectors or +size{K,M,G} (104857600-314572799, default 314572799):
    Using default value 314572799
    Partition 2 of type Linux and of size 100 GiB is set
    
    Command (m for help):
    ```

    表示分区完成。

11. 输入“p”，按“Enter”，查看分区的详细信息。

    回显类似如下信息：

    ```
    Command (mfor help): p
    
    Disk /dev/sda: 161.1 GB, 161061273600 bytes, 314572800 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x915ffe6a
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1            2048   104857599    52427776   83  Linux
    /dev/sda2       104857600   314572799    104857600  83  Linux
    
    Command (m for help):
    ```

12. 输入“w”，按“Enter”，将分区结果写入分区表中。

    回显类似如下信息，表示分区创建完成。

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

13. 执行以下命令，将新的分区表变更同步至操作系统。

    **partprobe**

14. 根据磁盘的文件系统，分别执行以下操作。
    -   若磁盘文件系统为ext\*，请执行以下步骤。
        1.  执行以下命令，检查磁盘分区文件系统的正确性。

            **e2fsck -f** _磁盘分区_

            命令示例：

            **e2fsck -f /dev/sda2**

            回显类似如下信息：

            ```
            [root@ecs-scsi ~]# e2fsck -f /dev/sda2
            e2fsck 1.42.9 (28-Dec-2013)
            Pass 1: Checking inodes, blocks, and sizes
            Pass 2: Checking directory structure
            Pass 3: Checking directory connectivity
            Pass 4: Checking reference counts
            Pass 5: Checking group summary information
            /dev/sda2: 11/3276800 files (0.0% non-contiguous), 251790/13107200 blocks
            ```

        2.  执行以下命令，扩展磁盘分区文件系统的大小。

            **resize2fs** _磁盘分区_

            命令示例：

            **resize2fs /dev/sda2**

            回显类似如下信息：

            ```
            [root@ecs-scsi ~]# resize2fs /dev/sda2
            resize2fs 1.42.9 (28-Dec-2013)
            Resizing the filesystem on /dev/sda2 to 26214400 (4k) blocks.
            The filesystem on /dev/sda2 is now 26214400 blocks long.
            ```

        3.  （可选）执行以下命令，新建挂载目录。

            若需要挂载至新建目录下，执行该操作。

            **mkdir** _挂载目录_

            以新建挂载目录“/mnt/test”为例：

            **mkdir** **/mnt/test**

        4.  执行以下命令，挂载磁盘分区。

            **mount** _磁盘分区_ _挂载目录_

            以挂载分区“/dev/sda2”至“/mn/test”为例：

            **mount /dev/sda2 /mnt/test**

            >![](public_sys-resources/icon-note.gif) **说明：**   
            >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。  


    -   若磁盘文件系统为xfs，请执行以下步骤。
        1.  （可选）执行以下命令，新建挂载目录。

            若需要挂载至新建目录下，执行该操作。

            **mkdir** _挂载目录_

            以新建挂载目录“/mnt/test”为例：

            **mkdir** **/mnt/test**

        2.  执行以下命令，挂载磁盘分区。

            **mount** _磁盘分区_ _挂载目录_

            以挂载分区“/dev/sda2”至“/mn/test”为例：

            **mount /dev/sda2 /mnt/test**

            >![](public_sys-resources/icon-note.gif) **说明：**   
            >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。  

        3.  执行以下命令，扩展磁盘分区文件系统的大小。

            **sudo** **xfs\_growfs** _磁盘分区_

            命令示例：

            **sudo** **xfs\_growfs** **/dev/sda2**

            回显类似如下信息：

            ```
            [root@ecs-scsi ~]# sudo xfs_growfs /dev/sda2
            meta-data=/dev/sda2              isize=512     agcount=4, agsize=3276800 blks
                     =                       sectsz=512    attr=2, projid32bit=1
                     =                       crc=1         finobt=0, spinodes=0
            data     =                       bsize=4096    blocks=13107200, imaxpct=25
                     =                       sunit=0       swidth=0 blks
            naming   =version2               bsize=4096    ascii-ci=0 ftype=1
            log      =internal               bsize=4096    blocks=6400, version=2
                     =                       sectsz=512    sunit=0 blks, lazy-count=1
            realtime =none                   extsz=4096    blocks=0, rtextents=0
            data blocks changed from 13107200 to 26214400df .
            ```


15. 执行以下命令，查看挂载结果。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-scsi ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  2.0G   39G   5% /
    devtmpfs       devtmpfs  509M     0  509M   0% /dev
    tmpfs          tmpfs     520M     0  520M   0% /dev/shm
    tmpfs          tmpfs     520M  7.2M  513M   2% /run
    tmpfs          tmpfs     520M     0  520M   0% /sys/fs/cgroup
    tmpfs          tmpfs     104M     0  104M   0% /run/user/0
    /dev/sda1      ext4       53G   55M   50G   1% /mnt/sdc
    /dev/sda2      ext4      106G   63M  101G   1% /mnt/test
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >云服务器重启后，挂载会失效。您可以修改“/etc/fstab”文件，将新建磁盘分区设置为开机自动挂载，请参见[设置开机自动挂载磁盘分区](#section1107170115310)。  


## 设置开机自动挂载磁盘分区<a name="section1107170115310"></a>

设置云服务器系统启动时自动挂载磁盘分区，不能采用在“/etc/fstab”直接指定设备名（比如/dev/vdb1）的方法，因为云中设备的顺序编码在关闭或者开启云服务器过程中可能发生改变，例如/dev/vdb1可能会变成/dev/vdb2。推荐使用UUID来配置自动挂载磁盘分区。

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



