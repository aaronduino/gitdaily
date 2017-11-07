# Day 42

You have not decided on any branch? Did you miss a reset git --hard? You have tested git filter-branch on a deposit with lots of super important patches?

    git reflog

Reflog records all the changes that are made on the branches and the
deposit. You should see by default your commits, merge and other sweater. A voucher
spy who can get you out of trouble.

Here is a typical exit from reflog.

    d2bbd0e HEAD @ {1}: commit: Run the bootstrap script when running bench.
    bd91916 HEAD @ {2}: bd919164c72c38b88a85275ee5b9add7f7a8f382: updating HEAD
    2ce209e HEAD @ {3}: pull origin master: Merge made by recursive.
    bd91916 HEAD @ {4}: commit: Generate tsung scenario from yml file.
    4cdc612 HEAD @ {5}: checkout: moving from complex_metadata to develop
    44fb6fc HEAD @ {6}: commit: Initial support of complex metadata in events.
    4cdc612 HEAD @ {7}: checkout: moving from 4cdc61204e4ea5c6814c65c88e2ef19031c2cf6d to complex_metadata

For example, to raprator a commit that is in any branch (* Not currently on any branch. *):

    git reflog (find the good commit, for example d2bbd0e)
    git checkout master
    git cherry-pick d2bbd0e

Or get your deposit after a git filter-branch:

    git reflog
    129b276 HEAD @ {0}: filter-branch: rewrite
    bbd8de8 HEAD @ {1}: rebase -i (pick): Optimize uce_paginate.
    git reset --hard bbd8de8

Some subcommands are available as * expire * and * delete *.

    git help reflog
