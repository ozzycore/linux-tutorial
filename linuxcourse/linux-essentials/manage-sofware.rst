Managing Software
+++++++++++++++++

Key Goals
=========
* Update local software/packages from remote/local repository

Content
=======
* yum:
   * yum cli
   * yum repository
   * yum cache
* rpm:
   * rpm cli

Useful Links
============
* RedHat docs - `Chapter 8. YUM: <https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system_administrators_guide/ch-yum>`_
* RedHat docs - `Appendix A. RPM: <https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system_administrators_guide/ch-rpm>`_


Exercises
=========
#. Install the 'epel' repository and disable it using yum cli.
#. Make sure the 'updates' repository is enabled (if not, enable it by editing it's repo file).
#. Find which package installs the 'netstat' command.
#. Print the information of that package.
#. List all the files that this package installs (full paths).
#. Find which rpm package installs the '/etc/hosts' file?
#. Explain the 'rpm -V <package_name>' command.
#. List all the available versions of 'httpd' package that available for installation.
#. Install the newest 'httpd' package available.
#. List all the installed packages that contains the 'kernel' word in the <package_name>.
#. List all the dependencies of the 'nmap' package.
#. Which command lists all the available [enabled & disable] repositories on your system?
#. Using yum, download (without installing) the 'tree' package. where is it stored (directory)?
#. Which command can be used for cleaning your current yum cache?
#. Which command can be used for rebuilding the yum cache?
#. Find how many packages (rpms) are installed on your system?
#. Explain what is a 'mirrorlist' and how is it related to yum?
