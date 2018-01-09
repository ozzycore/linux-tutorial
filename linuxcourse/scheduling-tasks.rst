scheduling-tasks
++++++++++++++++



Key Goals
=========
* Schedule tasks in order to run them at a spesific date and time.
* Verify completion of schedualed jobs
* Use scripting and automate system tasks

Content
=======
* crontab 
* /etc/crontab
* anacron
* at


Exercises
=========
crontab
~~~~~~~
#. Run: 'ls /etc/cron*' to explore the cron files. 

#. Using the following cron's syntax::

    # Example of job definition:
    # .---------------- minute (0 - 59)
    # |  .------------- hour (0 - 23)
    # |  |  .---------- day of month (1 - 31)
    # |  |  |  .------- month (1 - 12) OR jan,feb,mar,apr ...
    # |  |  |  |  .---- day of week (0 - 6) (Sunday=0 or 7) OR sun,mon,tue,wed,thu,fri,sat
    # |  |  |  |  |
    # *  *  *  *  * user-name  command to be executed

* Use cron's syntax (above) to write the answer:
    * Run the job every 10 min?
    * How would you run a task every day between sunday to friday at midnight time?
    * At 10 and 40 min of each hour?
    * Explain the following schedule task: 
        * 30 7-14 * * 1-5
        * \*/10 * * * 7

#. Scenario:
    #. Create a script that compresses your home directory and saves it in a non-root user home directory.
    #. With the root user edit /etc/crontab to schedule your task.
    #. Schedule a new task using 'crontab -e' to decompress that archive.
    #. Use crontab to list your jobs.
    #. Remove it after the task is done (use crontab command).
    #. Lets assume that the system is down in the execution time of that current job, when the job will be executed?

#. How can you manage a white list of users that are able to run cron's tasks?

anacron
~~~~~~~
#. On your laptop, would you run anacron or cron, explain why.
#. Explain the resulted scheduled task when appanding the following line to the bottom of the /etc/anacrontab::
    1    45    backup  tar -cf /tmp/backup /etc
#. How come there is a crond service for running the crontab jobs, but there is not an anacrond service, how anacron runs its jobs?

at
~~
#. When would you use an at job over corn?
#. Which service runs the at's jobs?
#. How can you black-list users from running at's jobs?













