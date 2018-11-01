File Systems
++++++++++++

Key Goals
=========

* Understand what a file system is.
* Different types of filesystems: ext[2-4], xfs, vfat (fat12, fat16, fat32), ios9660, swap.
* Create, tune, check and mount different file systems.


Content
=========

* File systems in general - what is it, purposes, structure
* Attributes of different file systems, comparison between them
* Journaling - what were the problems before it, different levels of journaling.
* Mounting - mounting in general, secure mounting, remote mounting.
* Relevant files - /proc/filesystems, /etc/filesystems, /proc/mounts, /etc/mtab, /etc/fstab
* The command line tools:
	* mkfs, mke2fs
        * tune2fs
        * fsck, e2fsck
        * mount (with secure options as well), umount

Exercises
=========

1. List the filesystems that are known by your system.
2. On a virtual machine:
	* Create an ext2 filesystem on a primary partition.
        * Create an ext3 filesystem on a logical drive.
        * Create an ext4 filesystem on a primary partition.
        * Create an xfs filesystem on a primary/extended partition.
        * Set the reserved space for root on the ext3 filesystem to a different value.
        * Verify your work with several tools.
        * Perform a file system check on all the new filesystems that you've added.....
3. On the same virtual machine:
	* Mount the ext2 filesystem on /home/@your_dir_name
        * Mount the ext4 file system on /mnt, copy some files to it from another directory, then umount it, mount it again as ro on /srv/nfs/@your_dir_name. Where are the files you copied?
        * Verify your work with several command line tools and file exploration.
        * Make one of the previous mounts permanent, reboot the machine to test that it works.
4. What happens when you mount a file system on a directory that already has some files in it?
5. What happens when you mount 2 different file systems on the same mount point?
6. Perform a file system check on the filesystem that is mounted on /srv/nfs/@your_dir_name.
