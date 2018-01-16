The Boot Process
++++++++++++++++

Key Goals
=========
* Understanding the Linux boot process
* 

Content
=======
* firmware:
    * BIOS
        * MBR
    * UEFI
        * GPT (GUID)
        * EFI system partitions (ESP)
        * UEFI native boot
        * Secure boot

* Bootloader:
    * grub & grub2

* initramfs 
    * cpio

* kernel (vmlinuz)

Useful Links
============
* https://www.happyassassin.net/2014/01/25/uefi-boot-how-does-that-actually-work-then/

Exercises
=========
cpio
~~~~
#. Scenario:
    #. Find the type of your /boot/initramfs-<version> file.
    #. Extract this file to /tmp/tempdir/
    #. Run tree to examin it's content
#. Scenario:
    #. Archive all the pdfs files inside your /usr/share/doc/ directory using cpio.
    #. Extract them to your local home directory.

dd
~~
#. Scenario:
    #. Run: lsblk, which partion is your /boot partition?
    #. Create a complete copy of your boot partition (name it boot.img)
#. Using dd, how would you wipe the /dev/sda disk?
#. Scenario:
    #. Run: fdisk -l which prints the Master Boot Recored (MBR).
    #. Backup the MBR
    #. Delete the MBR using dd
    #. Run the fdisk -l again, what is the result?
    #. Restore the MBR
    


    
Firmware - BIOS & UEFI
~~~~~~~~~~~~~~~~~~~~~~
* Where is the BIOS stored?
* Can someone make changes to the BIOS firmware?
* Is there some standart (like RFC) for the BIOS firmware?
* What the BIOS knows about our system?
* Note the main difference between the BIOS and UEFI role in the boot process?
* Can a UEFI firmware boot from an MBR formmatted disk?
* Explain what is a "Secure boot"




