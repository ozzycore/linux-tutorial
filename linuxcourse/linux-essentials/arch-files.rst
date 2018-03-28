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


Traning questions
=================
tar, gzip & gunzip, bzip2 & bunzip2
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#. Questions:
    #. What can you do with tar but can't do with gzip?
#. Scenario:
    #. Backup your home directory content to the /tmp/backup_user.tar (use tar).
    #. Use du (disk usage) to examine the size of your backup file. 
    #. Use du to calculate the sum of the actual files located inside your home directory.
    #. How much space did the compressing process save you and how much time did it take (use the time command)?
    #. Extract the /tmp/backup_user.tar file to the /opt/tempdir directory.
    #. remove /opt/tempdir directory.
    #. Use gzip to compress /tmp/backup_user.tar 
    #. How much space did the compressing process save you and how much time did it take (use the time command)?
    #. Unzip the file to tar again.
    #. Use bzip2 to compress /tmp/backup_user.tar 
    #. How much space did the compressing process save you and how much time did it take (use the time command)?
    #. Unzip the file to tar again.

