# Day 39

You want to rewrite your git history to group, delete, and generally change everything.

git rebase -i SHA1

SHA1 is the starting commit, which you do not want to change. All those at
above can be rewritten. Git opens your * EDITOR * and asks you what
operations you want to do. You can keep the commit as it is, the
merge with the previous one, delete it.

pick 379ab2a Move all presence as pid.
pick 42bab02 Update timeout module to use the new presence api.
pick d1da4b4 No more indexes for uce_presence_mongodb.
pick 94835c2 No more indexes for uce_presence_mnesia.
pick 0a481e9 Optimize uce_paginate.
pick 09b4224 Connected user as pid.

In the previous example, you can modify the buffer as follows:

pick 379ab2a Move all presence as pid.
squash 42bab02 Update timeout module to use the new presence api.
No more indexes for uce_presence_mongodb.
squash 94835c2 No more indexes for uce_presence_mnesia.
reword 09b4224 Connected user as pid.

What's going to happen :

* 42bab02, d1da4b4 and 94835c2 will be merged with 379ab2a. Git will also propose to rewrite the commit message.
* You will be able to rewrite the commit message of 09b4224.
* Since commit 0a481e9 is removed from the buffer, it will also be removed from the history.

git help rebase
