============
GIT & GITHUB
============
Git is a powerful tool vor version control. Github is a kind of git remote graphical user interface.

git
===
These are the basic and most important git command you have to type in your terminal:

* **clone** a repository (make a local copy on your computer)::

    git clone *url of the repository*
    
* if you have created, edited or removed some files in the repository, you have to **add** it::

    git add *name of the file/s*
    
in this way all your files will be put in the *staging area*

* now you can **commit** all your changes, this is, add a *message* to the edited files::

    git commit -m "message of the commit"
    
.. note:: many files can be inside the same commit. If you want to create different commit for different files, you have to add the files and write the commit in different steps
    
* once you have made the commit/s, the files are ready to be **pushed** in the main repository::

    git push
    
.. note:: you can always use :code:`git status` in order to see your job and understand all the steps

* you can also **pull** the changes (if some changes have been made) from the main repository and load them in your local one::

    git pull
    

Other useful command are:

* you can create a different **branch** of the repository and go inside it::

    git branch *name of the new branch*
    git checkout *name of the new branch*
    
    these commands can be merged in a single one
    
    git checkout -b *name of the new branch*
    
* *branches* are used when you want to add some pathes to the main code or create a similar (but different) release of it (for example all the QGIS releases are different brenches of the main master one). You can **merge** the branch with all the changes using::

    git merge *name of the branch*
    
* you can remove the the files you have put in the *staging area* with the :code:`git add` command::

    git reset HEAD
    
é you can have a look at the **log** and see the **differences** using::

    git log
    git diff


These are other useful references you can find:

`OverAPI <http://overapi.com/git/>`_
`gitref <http://gitref.org/basic/#reset>`_
`other referece <http://www.sbf5.com/~cduan/technical/git/git-1.shtml>`_
