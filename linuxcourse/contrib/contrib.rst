To Contribute
+++++++++++++

The following documentation is built on a Git based workflow. The following section will describe and guide you on how to make updates and contributions to this webpage using a Git based workflow, which will
include: pull request, continuous integration and delivery - NO prior Git experiance is assumed.

Before contributing, accomplish the following steps:

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



* Git clone the repository `Tech-Docs <https://github.com/ozzycore/tech-docs>`_.
* Run **make html** to build all the html files.
* Use pull requests to push your updates. 

* Use the `ReStructured Text markup syntax <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`_. :)
