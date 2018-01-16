Block Devices
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

* The command line tools:
    * fdisk
    * gdisk
    * parted

Exercises
=========
lsblk
~~~~~
* Add a new disk to your virtual machine:
    * Run lsblk, explain the MAJ and MIN value of your new device. 

fdisk
~~~~~


parted
~~~~~~
* Why would we use parted over fdisk or gdisk?
* mkpart extended 201 -1
* Can i have 13 logical partitions?

