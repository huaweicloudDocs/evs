# 扩展系统盘的分区和文件系统（Linux）<a name="evs_01_0072"></a>

## 操作场景<a name="section4385650719406"></a>

通过云服务管理控制台扩容成功后，仅扩大了云硬盘的存储容量，因此需要参考本章节操作扩展分区和文件系统。

对于Linux操作系统而言，需要将扩容部分的容量划分至已有分区内，或者为扩容部分的云硬盘分配新的分区。

如果在云服务器关机的时候扩容了系统盘，则开机后，Linux系统盘的新增容量可能会自动扩展至末尾分区内，此时新增容量可以直接使用。

本文以“CentOS 7.4 64bit”操作系统为例，提供growpart和fdisk两种工具的扩容指导，仅适用于弹性云服务器。不同操作系统的操作可能不同，本文仅供参考，具体操作步骤和差异请参考对应操作系统的产品文档。

扩展裸金属服务器系统盘的分区和文件系统，请参见[如何扩展快速发放裸金属服务器的根分区大小](https://support.huaweicloud.com/bms_faq/bms_faq_0062.html)。

-   [扩大已有MBR分区](#section9613733145218)
-   [新增MBR分区](#section9194153012119)

>![](public_sys-resources/icon-notice.gif) **须知：** 
>扩容时请谨慎操作，误操作可能会导致数据丢失或者异常，建议扩容前对数据进行备份，可以使用CBR或者快照功能，CBR请参见[管理备份云硬盘](管理备份云硬盘.md)，快照功能请参见[创建快照（公测）](创建快照（公测）.md)。

## 前提条件<a name="section51503350171737"></a>

-   已通过管理控制台扩容云硬盘容量，并已挂载至云服务器，请参见[扩容“正在使用”状态的云硬盘容量](扩容-正在使用-状态的云硬盘容量.md)或者[扩容“可用”状态的云硬盘容量](扩容-可用-状态的云硬盘容量.md)。
-   已登录云服务器。
    -   弹性云服务器请参见[登录弹性云服务器](https://support.huaweicloud.com/qs-ecs/zh-cn_topic_0092494193.html)。
    -   裸金属服务器请参见[登录裸金属服务器](https://support.huaweicloud.com/qs-bms/bms_qs_0004.html)。

-   Linux操作系统内核版本不低于3.6.0。

    您可以使用**uname -a**命令查看Linux内核版本。内核版本低于3.6.0时，请参考[扩展磁盘分区和文件系统（Linux系统内核低于3.6.0）](https://support.huaweicloud.com/bestpractice-evs/evs_02_0025.html)。


## 扩大已有MBR分区<a name="section9613733145218"></a>

以“CentOS 7.4 64bit”操作系统为例，系统盘“/dev/vda”原有容量40GB，只有一个分区“/dev/vda1”。将系统盘容量扩大至100GB，本示例将新增的60GB划分至已有的MBR分区内“/dev/vda1”内。

1.  （可选）执行以下命令，安装growpart扩容工具。

    **yum install cloud-utils-growpart**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >可以用**growpart**命令检查当前系统是否已安装growpart扩容工具，若回显为工具使用介绍，则表示已安装，无需重复安装。

2.  执行以下命令，查看系统盘“/dev/vda”的总容量。

    **fdisk -l**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# fdisk -l
    
    Disk /dev/vda: 107.4 GB, 107374182400 bytes, 209715200 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000bcb4e
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    ```

3.  执行以下命令，查看系统盘分区“/dev/vda1”的容量。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  2.0G   39G   5% /
    devtmpfs       devtmpfs  2.0G     0  2.0G   0% /dev
    tmpfs          tmpfs     2.0G     0  2.0G   0% /dev/shm
    tmpfs          tmpfs     2.0G  9.0M  2.0G   1% /run
    tmpfs          tmpfs     2.0G     0  2.0G   0% /sys/fs/cgroup
    tmpfs          tmpfs     398M     0  398M   0% /run/user/0
    ```

4.  执行以下命令，指定系统盘待扩容的分区，通过growpart进行扩容。

    **growpart** _系统盘 分区编号_

    命令示例：

    **growpart /dev/vda 1**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# growpart /dev/vda 1
    CHANGED: partition=1 start=2048 old: size=83884032 end=83886080 new: size=209713119,end=209715167
    ```

5.  执行以下命令，扩展磁盘分区文件系统的大小。

    **resize2fs** _磁盘分区_

    命令示例：

    **resize2fs /dev/vda1**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# resize2fs /dev/vda1
    resize2fs 1.42.9 (28-Dec-2013)
    Filesystem at /dev/vda1 is mounted on /; on-line resizing required
    old_desc_blocks = 5, new_desc_blocks = 13
    The filesystem on /dev/vda1 is now 26214139 blocks long.
    ```

6.  执行以下命令，查看扩容后系统盘分区“/dev/vda1”的容量。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-test-0001 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4      106G  2.0G   99G   2% /
    devtmpfs       devtmpfs  2.0G     0  2.0G   0% /dev
    tmpfs          tmpfs     2.0G     0  2.0G   0% /dev/shm
    tmpfs          tmpfs     2.0G  9.0M  2.0G   1% /run
    tmpfs          tmpfs     2.0G     0  2.0G   0% /sys/fs/cgroup
    tmpfs          tmpfs     398M     0  398M   0% /run/user/0
    ```


## 新增MBR分区<a name="section9194153012119"></a>

系统盘“/dev/vda”原有容量40GB，只有一个分区“/dev/vda1”。将系统盘容量扩大至80GB，本示例为新增的40GB分配新的MBR分区“/dev/vda2”。

1.  执行以下命令，查看磁盘的分区信息。

    **fdisk -l**

    回显类似如下信息：

    ```
    [root@ecs-2220 ~]# fdisk -l
    
    Disk /dev/vda: 85.9 GB, 85899345920 bytes, 167772160 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x0008d18f
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    ```

    表示当前系统盘“dev/vda”容量为80 GB，当前正在使用的分区“dev/vda1”为40 GB，新扩容的40 GB还未分配分区。

2.  执行如下命令之后，进入fdisk分区工具。

    **fdisk /dev/vda**

    回显类似如下信息：

    ```
    [root@ecs-2220 ~]# fdisk /dev/vda
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
    ```

    表示磁盘有两种分区类型：

    -   “p“表示主分区。
    -   “e“表示扩展分区。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >磁盘使用MBR分区形式，最多可以创建4个主分区，或者3个主分区加1个扩展分区，扩展分区不可以直接使用，需要划分成若干个逻辑分区才可以使用。
    >磁盘使用GPT分区形式时，没有主分区、扩展分区以及逻辑分区之分。

4.  以创建一个主要分区为例，输入“p”，按“Enter”，开始创建一个主分区。

    回显类似如下信息：

    ```
    Select (default p): p
    Partition number (2-4, default 2): 
    ```

5.  以分区编号选择“2”为例，输入分区编号“2”，按“Enter”。

    回显类似如下信息：

    ```
    Partition number (2-4, default 2): 2
    First sector (83886080-167772159, default 83886080):
    ```

6.  输入新分区的起始磁柱值，以使用默认起始磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    First sector (83886080-167772159, default 83886080):
    Using default value 83886080
    Last sector, +sectors or +size{K,M,G} (83886080-167772159,default 167772159):
    ```

7.  输入新分区的截止磁柱值，以使用默认截止磁柱值为例，按“Enter”。

    系统会自动提示分区可用空间的起始磁柱值和截止磁柱值，可以在该区间内自定义，或者使用默认值。起始磁柱值必须小于分区的截止磁柱值。

    回显类似如下信息：

    ```
    Last sector, +sectors or +size{K,M,G} (83886080-167772159,
    default 167772159):
    Using default value 167772159
    Partition 2 of type Linux and of size 40 GiB is set
    
    Command (m for help): 
    ```

8.  输入“p”，按“Enter”，查看新建分区。

    回显类似如下信息：

    ```
    Command (m for help): p
    
    Disk /dev/vda: 85.9 GB, 85899345920 bytes, 167772160 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x0008d18f
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/vda1   *        2048    83886079    41942016   83  Linux
    /dev/vda2        83886080   167772159    41943040   83  Linux
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

    表示分区创建完成。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果之前分区操作有误，请输入“q”，则会退出fdisk分区工具，之前的分区结果将不会被保留。

10. 执行以下命令，将新的分区表变更同步至操作系统。

    **partprobe**

11. 执行以下命令，设置新建分区文件系统格式。

    **mkfs** **-t** _文件系统_ _磁盘分区_

    -   ext\*文件系统命令示例：

        以“ext4” 文件格式为例：

        **mkfs -t ext4 /dev/vda2**

        回显类似如下信息：

        ```
        [root@ecs-2220 ~]# mkfs -t ext4 /dev/vda2
        mke2fs 1.42.9 (28-Dec-2013)
        Filesystem label=
        OS type: Linux
        Block size=4096 (log=2)
        Fragment size=4096 (log=2)
        Stride=0 blocks, Stripe width=0 blocks
        2621440 inodes, 10485760 blocks
        524288 blocks (5.00%) reserved for the super user
        First data block=0
        Maximum filesystem blocks=2157969408
        320 block groups
        32768 blocks per group, 32768 fragments per group
        8192 inodes per group
        Superblock backups stored on blocks:
                32768, 98304, 163840, 229376, 294912, 819200, 884736, 1605632, 2654208,
                4096000, 7962624
        
        Allocating group tables: done
        Writing inode tables: done
        Creating journal (32768 blocks): done
        Writing superblocks and filesystem accounting information: done
        ```

    -   xfs文件系统命令示例：

        **mkfs** **-t** **xfs** **/dev/vda2**

        回显类似如下信息：

        ```
        [root@ecs-2220 ~]# mkfs -t xfs /dev/vda2 
        meta-data=/dev/vda2              isize=512     agcount=4, agsize=2621440 blks
                 =                       sectsz=512    attr=2, projid32bit=1
                 =                       crc=1         finobt=0, sparse=0
        data     =                       bsize=4096    blocks=10485760, imaxpct=25
                 =                       sunit=0       swidth=0 blks
        naming   =version2               bsize=4096    ascii-ci=0 ftype=1
        log      =internal log           bsize=4096    blocks=5120, version=2
                 =                       sectsz=512    sunit=0 blks, lazy-count=1
        realtime =none                   extsz=4096    blocks=0, rtextents=0
        ```

    格式化需要等待一段时间，请观察系统运行状态，若回显中进程提示为done，则表示格式化完成。

12. （可选）执行以下命令，新建挂载目录。

    若需要挂载至新建目录下，执行该操作。

    **mkdir** _挂载目录_

    以新建挂载目录“/opt”为例：

    **mkdir /opt**

13. 执行以下命令，挂载新建分区。

    **mount** _磁盘分区_ _挂载目录_

    以挂载新建分区“/dev/vda2”至“/opt”为例：

    **mount /dev/vda2 /opt**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >新增加的分区挂载到不为空的目录时，该目录下原本的子目录和文件会被隐藏，所以，新增的分区最好挂载到空目录或者新建目录。如确实要挂载到不为空的目录，可将该目录下的子目录和文件临时移动到其他目录下，新分区挂载成功后，再将子目录和文件移动回来。

14. 执行以下命令，查看挂载结果。

    **df -TH**

    回显类似如下信息：

    ```
    [root@ecs-2220 ~]# df -TH
    Filesystem     Type      Size  Used Avail Use% Mounted on
    /dev/vda1      ext4       43G  2.0G   39G   5% /
    devtmpfs       devtmpfs  509M     0  509M   0% /dev
    tmpfs          tmpfs     520M     0  520M   0% /dev/shm
    tmpfs          tmpfs     520M  7.2M  513M   2% /run
    tmpfs          tmpfs     520M     0  520M   0% /sys/fs/cgroup
    tmpfs          tmpfs     104M     0  104M   0% /run/user/0
    /dev/vda2      ext4       43G   51M   40G   1% /opt
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



