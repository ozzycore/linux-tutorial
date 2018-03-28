File Permissions
++++++++++++++++

.. basic file systems: xfs, ext (acl difference), show the mounted (useing mount) grep the root one, say lvm


Key Goals
=========
* Listing file permissions
* Modifing standart file permissions
* Changing the default system permissions
* Changing file ownership

Content
=======
Listing permissions:
    * stat
Changing default system permissions:
    * umask
File permissions:
    * chmod
    * Sticky bit
    * GroupID bit
    * UserID bit
    * getfacl
User permissions:
    * chown
    * chgrp
    * id
    * primary and secondary groups


Exercises
=========
#. The following prints the file permission of the /etc/host file::

     -rw-r--r--. 1 root root 288 Oct 25 23:20 /etc/hosts

   * Explain the file permission structure.
   * Which parameter indicates us about the type of a file?
   * Which file types are exists in the linux environment?

#. Use stat to examine the '/etc/hosts' it full file permissions.
#. Which command will set our default system permissions into 640 (use umask)?
#. Which command will ser our default system permissions into -rw------- (use umask)?
#. Are the file system permission cumulative? explain what is a cumulative permissions.
#. Explain what is the sticky bit? and what it controls?
#. Explain the usage of the GroupID and UserID bit.
#. Run 'ls -l /usr/bin/passwd', explain it's file permissions.
#. List all the user's groups using the id command.
#. Explain the purpose of the 'wheel' group in a linux evironment.
#. Why there is a seperation to a primary and secondary groups, why it can not be just a set of groups?
#. How can we change our primary group?
#. How would you change the user and group ownership for all the content of a directory (recursively).
#. Are the permissions copied while someone copies a file? how can we control that? 
#. Which kind of permission are needed in oreder to copy some file from it's current location to a new one?
#. Scenario:
    * Inside your local home directory, create a stickydir directory with a sticky bit on.   
    * Inside stickydir, create file1 file that contains the following content: "Hello World".
    * Change the permissions to -rw------- (use the numeric notation).
    * Add an execute permissions to the group (use the symbolic notation).
    * Set 'no permissions' to others (use '=' sign).
    * Change file's group to 'wheel'.






