RAID
+++++++

Key Goals
=========

* Understanding the concept of RAIDs and learn about their different types.
* Create and manage software raid.

Contents
=========

* Striping.
* RAID - Hardware/Software RAID.
* Different RAID levels: RAID 0-6, RAID 10/01, RAID 50.
* fd partitions
* Relevant files: /proc/mdstat
* mdadm command.


Exercises
=========

1. * Add 3 virtual disks of 1GB each to a virtual machine.
   * Create a software raid 5 on the 3 disks.
   * Verify with fdisk and by exploring /proc/mdstat that the raid5 exists.
   * Stop and remove the raid 5.
   * Do the same thing for raid 1 with 2 virtual disks.
2. Why Does raid 5 is faster than raid 3/4?
3. How many minimum disk drives are required for R0, R1, R2, R3, R4, R5, R10 and R01.
4. What is the main difference between a software raid and hardware raid?
5. Which is the best RAID for performance and which is the best for redundancy?
