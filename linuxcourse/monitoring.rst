Basic Monitoring Tools
++++++++++++++++++++++

Key Goals
=========
* Monitor our system performance

Content
=======
* The procps-ng package:
    * free
    * df
    * top
    * vmstat
    * pgrep
    * pkill
    * pmap
    * ps
    * skill
    * slabtop
    * tload
    * uptime
    * vmstat
    * w & who
    * watch



Exercises
=========
#. Use the rpm tool to list all the tools that the procps-ng package installs (at /usr/bin).
#. List the available RAM in GB.
#. List the file system usage.
#. List all the pids of the sshd daemon.
#. Explain the 'pmap $$' output.
#. Which command enables you to view the number of cpus on your machine?
#. Run: uptime, explain the 3 seaction of the load avarage.
#. If i got 4 cpus on the machine and the load_avarage equals to 0.1, 2.5, 5.8, am i queuing cpu requests?
#. Run: cat /proc/uptime, exaplain what each column represents.
#. Using watch run uptime and refresh the output every 3 seconds.
#. Scenario:
    #. Use a virtual machine with 1 cpu.
    #. Run tload
    #. On a new shell, start compressing all the content of /usr/share/doc using bzip.
    #. When the cpu starts queuing tasks?
