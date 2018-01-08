The Boot Process
++++++++++++++++
* Understanding the Linux boot process
* 

Key Goals
=========
* cpio


Content
=======



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
    

    



