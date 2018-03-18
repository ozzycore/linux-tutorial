User and Group Managment
++++++++++++++++++++++++

Key Goals
=========
* Managing users' and groups' (local) life cycle
* Manage passwords
* Identify linux users

Content
=======
* Identify linux users:
    * id

* Managing users:
    * /etc/passwd
    * useradd
    * usermod
    * userdel
    * chsh

* Managing users' passwords:
    * /etc/shadow
    * passwd
    * chpasswd
    * chage

* Users's defaults:
    * /etc/login.defs

* Managing groups:
    * /etc/group
    * groupadd
    * groupmod
    * groupdel
    * newgrp
    * chgrp
 
* Managing groups' passwords:
    * /etc/gshadow
    * gpasswd


Exircises
=========
* Use the above commands to:
    * Create: user1, user2
    * Create a password for user1.
    * Create: group1, group2
    * Assign user1 to group1 and group2
    * List user1's secondary groups
    * Create a password for group2.

* In which usecase would someone run `chmod g+s` against some new dirctory?

* Modify the `/etc/skel` directory to contain some new files and verify it by creating a new user - user1.
* Why the `/etc/passwd` doesn't contain the users' passowrds?

