Version Control
===============

Why do we need version control? Isn't a file server where everyone just uploads new source 
code to enough? What about

* Synchronization across the team? Especially when working on the same file?
* Undoing short-term or long-term changes? You might be able to Crtl-z your way out of the last 10 edits but what about going back to that code you wrote about two months ago?
* Who changed *what*?
* All changes that are uploaded to the server are final. What if you want to send someone some early beta code?

The industry answer to this is **version control**. A version control system keeps track of the different versions of a 
file (*duh*). In doing so it can provide tremendous value to you as a developer by keeping your projects synchronized, 
giving you the ability to work on a feature, switch back to another version of the code and work on another feature, and 
transparently share these changes with your peers. You can also easily roll back to a previous version. 

**git** has become the *de-fact* standard for version control systems. Initially developed for the linux kernel it has 
wide acceptance in the open-source community and with corporations.

So popular in fact that GitHub has build a $7.5bn business out of hosting git repositories.

.. figure:: _static/nerdstagram.jpeg
    :width: 70%
    :align: center

A primer on git
^^^^^^^^^^^^^^^

Before diving into git lets define some terms we will use 

* **Repository** A repository stores a project within the context of git. It is a folder that contains all the files as well as all the meta information used by git. This information is saved in a folder called `.git`.
* **Commit** A commit is the fundamental "unit of change" for git. A commit contains all information on how the files that have been *added* to the commit have been changed compared to the previous version. Starting from the initial commit (and following this chain of changes) we can thus get the current version of the file. Each commit has a *hash value* attached to it that uniquely identifies the commit.
* **Branch** A branch is a *set of commits*. Every project will have at least one *master* branch but the ease of branching in git makes it possible to have a lot of branches. It is very typical to have a master branch - a *develop* branch for the current (somewhat) stable development version and branches for each feature that is being developed.
* **Diff** A diff lists all the changes that have been applied to a file. It can be used to show the changes since a file has last been comited or show changes that orcured between commits.
* **Merge** A merge is the process of combining two branches into each other. The big innovation of git was to make merging branches so simple that it became feasible to have a ton of them.
