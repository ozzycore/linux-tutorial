Block Devices and Partition Tables 
++++++++++++++

Key Goals
==========
* Listing block devices
* Block devices names
* List, add, remove and modify storage partitions
* Scripting partition creation


Content
=======
* Block devices
    * lsblk
* Partition tables
    * types:
        * MBR/msdos
        * GPT/GUID
    * primary partition, extended partition, logical partition
    * /proc/partitions, /proc/devices.
* The command line tools:
    * fdisk
    * gdisk
    * parted
    * sfdisk, partprobe

Exercises
=========

~~~~~
lsblk
~~~~~
* Add a new disk to your virtual machine:
    * Run lsblk, explain the MAJ and MIN value of your new device. 

fdisk
~~~~~
* Use fdisk to find the total size of all hard disk devices on your system.
* On a virtual machine (you can use VirtualBox/virt-manager for it) make a virtual machine, stop it, and then add two virtual 2 gigabytes scsi hard disk devices and 2 virtual 500 megabytes ide/ATA hard disk
  devices. 
	* Verify that you can see the disk devices in /dev and use fdisk with grep to display their total size.


parted
~~~~~~
* Why would we use parted over fdisk or gdisk?
* mkpart extended 201 -1
* Can i have 13 logical partitions?

partitions
~~~~~
* Use fdisk -l/df -h to display existing partitions and sizes and compare the outout between them.
* Make a VM with 2 virtual hard disks (A big one and a small one). On the small disk create a 500MB primary partition, and on the big disk create a 600MB primary partition and 2 200MB Logical drives.
* Use fdisk -l/ df -h to verify your work. Once again compare the output between the commands - do both commands display the new partitions?
* Create a backup with dd of the mbr that contains your 500MB primary partition and another backup for the partition table of the big disk, remove all your partitions with fdisk and restore them with your
  backups. (Do not use dd for the second backup, think why).

