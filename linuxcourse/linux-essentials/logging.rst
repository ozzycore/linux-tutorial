Linux Logging
+++++++++++++

Key Goals
=========
* Mointor login events
* Audit sudo and su system execution
* Using 'awk' to analyzing logs
* Rotate system's logs

Content
=======
* Main file (/var/log)
    * message
    * secure
    * audit
    * btmp & wtmp

* Logging commands
    * lastlog
    * last
    * lastb
    * journalctl
* rsyslog 
    * syslog
    * logger

* Log rotation
    * logrotate

Exercises
=========
Log files
~~~~~~~~~
* Which file considered to be the main logging file?
* Explain the difference between last and lastb command and thier correlation to the btmp and wtmp files.
* Scenario:
    * Which file contains information about the su and sudo events?
    * Print only the sudo events in the following format: *Date: <date> User: <user>.*
        * Use 'awk' command.
        * Use only the last 100 lines of the log file.
* What the journalctl command prints (by default)?
* Print all the logs since the last boot (using journalctl).

Rsyslog
~~~~~~~
* Explain the difference between rsyslog and syslog.
* The following rules located in the /etc/rsyslog.conf file, explaint thier meaning:
    * \*.emerg                                                 :omusrmsg:\*
    * \*.info;mail.none;authpriv.none;cron.none                /var/log/messages
* What is a facility?
* Scenario:
    * touch the following file /var/log/templog
    * Add the following rule to the /etc/rsyslog.conf file: *local1.info /var/log/andrew*
    * Restart rsyslog
    * Test your rule (using using the logger command).

Logrotate
~~~~~~~~~
* Which service runs the logrotate commands?
* Continue scenario:
    * Rotate the /var/log/templog log file, use the following configs:
        * Rotate the file when it's size gets to 10 bytes.
        * use compression
        * Dont rotate if the file is empty
        * Use the 'missingok' option
    * Use the logrotate command to rotate the log.





