Login Scripts
+++++++++++++

Key Goals
=========
* Understand login script role and usage 
* Managing template user environmet
* Login and non-login shells

Content
=======

Shells:
    * login shell
    * non-login shell

Login scripts:
    * /etc/bashrc
    * /etc/profile
    * /etc/profile.d
    * ~/.bashrc
    * ~/.bash_login
    * ~/.profile
    * ~/.bash_profile
    * ~/.profile

Logout scripts:
    * ~/.bash_logout

User tamplate home directory:
    * /etc/skel

Exercises
=========
* Scenario:
    * Run **su -**
    * Examine the output of: 
        * shopt login_shell
        * pwd
        * id
        * echo $USER

    * Run **su**
    * Examine the output of: 
        * shopt login_shell
        * pwd
        * id 
        * echo $USER
    * What is the differece between running *su* and *su -* ?

* List the order of execution of the login scripts when executing:
    * A login shell
    * a non-login shell
    * TIPS:
        * Add to the end of each file **echo <file_name>** and preform the logins.
        * Use **man bash**
    
* Which file **(~/.bashrc or ~/.bash_profile)** would you use in order to appand a new directory to the **PATH** variable: 
    * Like: **PATH = $PATH:/<new_directory>/**

* Scenario:
    * What is defined by the PS1 variable?
    * Which login script sets your PS1 variable?
    * Change it to "[\\u\@\\h \\w]\\$ " 

* Is there a point to **export** a variable inside of the ~/.bashrc file?

* What is the role of the **/etc/skel** directory?

