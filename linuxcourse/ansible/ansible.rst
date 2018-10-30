Ansible
+++++++

Content
=======
* Ansible - configuration management and automation tool.

Useful Links
============
* In order to start with Ansible, read the following sections of `Ansible Introduction <http://docs.ansible.com/ansible/latest/intro.html>`_:
    * Installation
    * Getting Started
    * Inventory
    * Introduction To Ad-Hoc Commands

* Read `How Ansible works? <https://www.ansible.com/overview/how-ansible-works>`_.

* Complete the Playbooks section of ansible's documentation: `Ansible Playbooks: <http://docs.ansible.com/ansible/latest/playbooks.html#>`_.

* Use this github repository as a reference for some examples and best practices for building `Ansible Playbooks <https://github.com/ansible/ansible-examples>`_.

NOTE: It is better to read the documentation while practicing writing some playbooks.

Exercises
=========

Theoretical Part
----------------
* How is Ansible different than other tools like Chef or Puppet?
* What is YAML?
* What is `when` and how do you use it?
* How do you extend a conditional over multiple tasks without defining the `when` conditional multiple times.
* How do you use blocks?
* How do you include tasks from external files?
* What is the diffrence between an include and a import?
* How do you pass variables at the command line?
* How do you ask for variable prompt?
* Why is a bad idea to commit secret data into a git repository?
* What are some of the ways to keep secret data out of a repository (Using Ansible)?
* What are the advantages and downsides of Ansible Vault?
* Where would you save Ansible configurations?
* Where is the best place to look for documentation about an Ansible module?
* How do you install a yum package using Ansible?
* How does Ansible indicate if something changed?
* Where are some places variables can be registered?
* How are variables referenced?
* How do you loop over an list or dictionary in Ansible?
* How do you define dependencies between roles?
* Why would you use the omit filter?
* Why would you use a mandatory variable in Ansible? and how do you define them?
* What is the usage of the `assert` module?
* What is a handler?
* What are the benefits of a role over a playbook?
* Where would use save your variables when you are writing a role?
* Why would you create more than one file in the tasks directory when you're writing a role?

Practical Part
--------------
* Install Ansible on your local machine.

* Scenario:
    * Provision 1 virtual machine that contains 3 block devices - 10G each.
    * Using Ansible from you local machine, provision on the remote:
        * Volume group - vgans01, that contains all three disks.
        * Create 2 logical volumes - lvans01, lvans02 (15G each).
        * Create a file system - xfs, on each one of them.
        * Create the following directories: dir01, dir02.
        * Mount dir01 to lvans01 and dir02 to lvans02.
     
