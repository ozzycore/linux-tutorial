To Contribute
+++++++++++++

The following documentation is built on a Git based workflow. This section will guide you on how to make updates and contributions to this web site.

.. note:: NO prior Git experiance is assumed.


Git clone the repository `Tech-Docs <https://github.com/ozzycore/tech-docs>`_, and follow the next steps::

        # Git clone
        $ git clone https://github.com/ozzycore/tech-docs

        # Check that you are on 'master'
        $ git branch
        > * master

        # Git check out to a new branch
        $ git checkout -b <new_branch>

        # Check that you are located on your new created branch - <new_branch>
        $ git branch
        > * <new_branch>
            master

Now, make the required changes, and continue::

        # Git add the changes
        $ git add <file_name> 
        # OR just 'git add' everything by running
        $ git add .

        # Git commit the changes
        $ git commit -m <commit message>

        # Push your local branch to the github
        $ git push origin <new_branch>

To create a pull request, login to the github repository using the browser, and create pull request to the 'master' branch. Your contribution will be merge after someone reviews and accepts your pull request.


.. note:: Please use the Sphinx's documentation for the syntax


You can se the `ReStructured Text markup syntax <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`_. :)

.. warning:: The following section is not required, you can use it to generate the html files and testing them before pushing to the remote git.
Accomplish the following steps:

* Provision a virtual machine - it is optional, you can use your local one.
* Install the prerequisites:
    * Python
    * Sphinx
    * The ReadTheDocs theme


Code::

        # Install python
        yum install python
        
        # Install pip
        yum install python2-pip
        
        # Install Sphinx
        pip install sphinx

        # Install The ReadTheDocs theme
        pip install sphinx-rtd-theme-0.2.4



* For the root of the git cloned repository, run **make html** to build all the html files.
* Install some webserver, for example: httpd, and access these generated html files for testing.

