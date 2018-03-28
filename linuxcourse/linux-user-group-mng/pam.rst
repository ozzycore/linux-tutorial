PAM
+++

Key Goals
=========
* Configure PAM
* Configure user resource limits
* Manage user processes
* Home dirs while logins
* Password policies
* Control login times

Content
=======
* Pam modules

Exercises
=========
Pam modules
-----------
* Explain what are PAM modules? note, what is the responsability of Pam modules and explain on which resources they have control?
* Where can you find these Pam modules on your system (directory)?
* What is the meaning of the `*.so` type of file?
* Modify Pam to create a home direcotry for a new user on login.
* Modify Pam to define a new password policy that enforces 8 charchters for each password.
* Use the `/etc/security/limit.conf` file to limit the users to maximum of 10 concurent processes. Test your work by running: 

```
#!/bin/bash
echo "Test"
$0 (it's the script name)
```


