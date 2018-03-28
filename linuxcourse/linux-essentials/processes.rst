Linux Processes
++++++++++++++++

Key Goals
=========
* Listing the running processes
* Identifing the resource utilization by process
* Moving tasks to backgroud / foregroud
* Killing processes
* Changing the process priority

Content
=======
Listing processes:
    * The /proc directory
    * ps
    * pstree
    * pgrep
    * top

Killing processes:
    * kill and pkill

Foregrouding & Backgrouding jobs:
    * bg
    * fg
    * jobs

Process priority:
    * nice
    * renice

Exercises
==========
#. Scenario:
    #. Run sleep 10000.
    #. How can you move it to the backgroud?
    #. How would you start it in a background initialy?
    #. Run sleep 10000 again (start it in a backgroud).
    #. Repeat it again.
    #. Run jobs to view the running tasks, what is the meaning of the + sign?
    #. Move the second one to the foreground and stop it.
    #. Terminate the other 2 using the kill command.

#. Explain the content of the /proc directory.
#. Which process is repesented by the following directory "cd /proc/$$"?
#. List the process details with a ProcessID equals to 1, which one is it?
#. What is the RSS (Resident Set Size), and how can we list it using the ps command?
#. Use ps and grep to list the sshd daemon.
#. List all the available signals that can be sent by kill.
#. Explain the difference between SIGKILL and SIGTERM.
#. Find your sshd pid and use kill to send it a SIGKILL signal.
#. Run top and sort it by %MEM (RAM) utilization.
#. Using pstree print the process tree of the NetworkManager service.
#. Scenario:
    #. Run sleep& 1000 three times in your bash shell.
    #. Use pgrep to list thier pids
    #. Use pkill to kill those processes
  
#. How can we view the Priority(PRI) and Nice(NI) values of a process?
#. Explain the meaning of the Nice(NI) value of a process ,and how is the CPU Priority(PRI) value is related to the NI value of a particular process?
#. What is the default values of Priority(PRI) and Nice(NI) variables for a new process?
#. What is the range of possible values that Priority(PRI) and Nice(NI) can have?
#. Run the 'sleep 1000' in a backgroud with the lowest possible Priority.
#. What is the usage of the renice command?

