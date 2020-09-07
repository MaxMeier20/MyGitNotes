* Find out storage / available diskspace: `df -h`    
* Format a drive
    1. Find the drive name (i.e. sdc1) with `df -h`
    2. Unmount the drive with `umount /dev/sdc1`
    3. Create a files system and label it "USB Drive" i.e.  `mkfs.ext4 /dev/sdb1 -L "USB Drive"`

    Sytem | System | System
    ----- | ----- | -----
    mkfs.bfs| mkfs.ext2 | mkfs.hfs |
    mkfs.msdos | mkfs.xfs | mkfs.btrfs
    mkfs.ext3  |    mkfs.hfsplus |  mkfs.ntfs      
    mkfs.cramfs  |  mkfs.ext4  |    mkfs.jfs 
    mkfs.reiserfs  | mkfs.exfat |    mkfs.fat
    mkfs.minix |     mkfs.vfa
* Identify active terminal emulator `ps -o 'cmd=' -p $(ps -o 'ppid=' -p $$)` or `pstree -sA $$ | head -n1 | awk -F "---" '{ print $(NF-1) }'`
* Identify running Linux / OS, easiest way is just installing `neofetch` (and appending that to the `.bashrc` so you see it always)
    * Distribution: `cat /etc/*-release` 
    * Kernel: `uname -a`or `uname -mrs`
* Shutdown the system cleanly and immediately `shutdown -h now` if the machine hangs try first `systemctl --force poweroff` (on systemD systems) and than `echo o >/proc/sysrq-trigger` <-- Both are just as dangerous as unplugging the cord for the filesystem, but avoid the electric charge on the mainboard

