Consoles & The Command Line (CLI)
+++++++++++++++++++++++++++++++++

Key Goals
=========
* Manage and access different consoles in linux
* Basic commands to navigate the command line

Content
=======
#. Consoles:
     * Consoles types:
         * Physical TTY
         * Local Pseudo TTY
         * Remote Pseudo TTY
     * Related commands:
         * tty
         * who

#. Command line basics:
    * Shortcuts
    * Related commands:
        * pwd
        * ls
        * tree
        * cd
        * exit

#. Wildcards

Exercises
=========
Consoles
~~~~~~~~
#. Explain the difference between Physical, Local Pseudo and Remote Pseudo TTY.
#. ssh is example to which kind of TTY?
#. How many physical consoles exist in a Linux environment?
#. Which shortcut can you use to bring up the physical TTY?
#. Run the tty command and explain it's output.
#. What is the meaning of the number of files in the /dev/pts directory?

The Command Line
~~~~~~~~~~~~~~~~
#. Explain the following CLI shortcuts:
    * CTL + l
    * CTL + r
    * CTL + w
    * CTL + d
#. Which shortcut makes the CLI's font bigger?
#. The cd command
    * How can you get to your home directory using cd?
    * Why would someone run the cd with the '-' option?
#. The who command:
    * Login to your second physical tty
    * Run the who command, exaplain the meaning of the output.
    * The ouput should contain :0, pts/0 and tty2, explain thier meaning.
#. The ls options:
    * List all the files in the /etc directory (including the hidden files).
    * List the files in the /etc directory so the most recently modified files are shown last.
    * Which functionality adds the -F option?
#. In the follwing example: ls -l $(tty), which functionality provides the '$(<command>)' 

Wildcards
~~~~~~~~~
#. Explain what is a wildcard.
#. !!
#. !$
#. List the directories that match the following conditions:
    * Located inside your home directory
    * Directory name starts with the 'D' character
#. List the files that match the following conditions:
    * Located inside /dev directory 
    * File name starts with sda and then followed by a single character (for example: /dev/sda8)
#. List only the following 2 files: /dev/sda1 and /dev/sda2 using a the [] wildcard.




