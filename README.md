# mlph_group_work

## Beginning guidelines
<!-- Making some changes and opening a pull request -->


### 1a: Fork the repository

Since you don't have write access to this repository, and also we want things simpler, the first step will be to make a "fork" of the repository.
This is basically a copy of the main repository, but one that you have complete control to modify as you see fit
(and that is visible to everyone else on GitHub).  Make sure you are logged in to GitHub, then go to the
repository and click the 'Fork' button.


### 1b: Clone your fork

Now that you have forked your repository, you can clone it to your computer using:

    git clone -o <username> https://github.com/<username>/mlph_group_work

Be sure to replace ``<username>`` with your GitHub username!

### 1c: Familiarize yourself with the code

Once the repository has been cloned, ``cd`` into it and check what files are available:

    cd mplh_group_work
    ls

You should now see the following files:

* ``README.md``: basic documentation for some of the code
* ``Task``: folder for respective exercises

<!-- * ``simple_functions.py``: a set of simple functions that should work properly

* ``buggy_function.py``: a function that contains one or more bugs -->


Take a look at these files, and familiarize yourself with the contents.

### 1d: Make a new branch

By default, you will be looking at the ``main`` "branch" of the repository. You're going to make some
changes to the code, but who knows... maybe the reviewers will spend so long reviewing your changes
that you want to do another set of unrelated changes in the mean time. Thus it's always best to make
changes in a dedicated branch. So before you make any changes, make a new branch with:

    git branch <name-of-branch>

You can then switch to this branch with:

    git checkout <name-of-branch>

Note that you can also write ``git checkout -b <name-of-branch>`` as a short-hand for the above two
commands. Branch names should be kept simple and reasonably short, and can't include e.g. spaces.

### 1e: Make some changes

At this point, you can implement changes in the code or add your codes.

### 1f: Commit the changes and push it to your fork

Now that you've made changes, the next step is to commit these changes to the repository. You can see
what files have changed since the last commit with:

    git status

We now need to 'stage' files before committing them - the difference between staging and committing
files is that staging consists of selecting which files you will want to commit changes for (you may
want to separate the commits for changes to different files for some reason). To stage files, use
the ``git add`` command as:

    git add file-to-stage

and repeat this for each file you want to include in the next commit. You can use ``git status``
to check which files have been staged for committing. Once you are happy with the files that have been
staged, you can create a commit in the repository using:

    git commit -m "Message describing the changes here"

Be sure to edit the commit message to be descriptive, so that anyone looking at the git history has
an idea of roughly what each commit does.

**Good commit message:** ``Fixed bug in this_function which was due to an off-by-one error``

**Bad commit message:** ``Fixed stuff. It's Friday evening and I want to go home now``

<!-- You can now check that your commit is in the history using:

    git log -->

If the commit is there, you are now ready to push your changes to GitHub! You can do this using:

    git push <username> <name-of-branch>

If this succeeds, you are ready for the next step. If you get an error about the changes being rejected,
ask your friendly stackoverflow or the creator of repo!

### 1g: Open a pull request

At this point, go to your fork on GitHub at ``https://github.com/<username>/mplh_group_work``, 

Click on **Compare & pull request**. 

At this point, give your pull request a sensible title, and use the description box to describe what
changes you've made, why you made them, and you can also mention if there are any unresolved issues for
 example. You can also preview the changes by scrolling down on the page.

If for some reason you don't see the yellow banner (for example, if you went and did something else
after pushing so that it timed out), you can also make a pull request by choosing your branch from the
drop-down menu and then choosing 'New pull request'

Once ready, hit **Create pull request**, and you're done!


The repo manager will review the changes and publish them.

Happy solving!
