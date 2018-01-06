Archiving Files
+++++++++++++++

Key Goals
=========
* Learn abount archiving and compressing files

Section Objectives
==================
* tar
* gzip & gunzip
* bzip2 & bunzip2
* cpio
* dd (disk duplicator)


Traning questions
=================
tar, gzip & gunzip, bzip2 & bunzip2
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#. Scenario:
    #. Backup your home directory content to the /tmp/backup_user.tar (use tar).
    #. Use du (disk usage) to examin the size of your backup file. 
    #. Use du to calculate the sum of the actual files located inside your home directory.
    #. How much space the compressing process saved you and how much time did it take?
    #. Extract the /tmp/backup_user.tar file to the /opt/tempdir directory.
    #. remove /opt/tempdir directory.
    #. Use gzip to compress /tmp/backup_user.tar 
    #. How much space the compressing process saved you and how much time did it take?
    #. Unzips the file to tar again.
    #. Use bzip2 to compress /tmp/backup_user.tar 
    #. How much space the compressing process saved you and how much time did it take?
    #. Unzips the file to tar again.

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
    

    



