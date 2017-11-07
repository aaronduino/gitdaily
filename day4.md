# Day 4

I want to change my last commit, because I put a bad
commit message.

    git commit --amend

Modifies the last commit message. Can also add the
changes to your staging area.

    git add myfile.erl && git commit --amend

Add the modification of myfile.erl in the previous commit.

This command rewrites the history git, you should NOT do it
if you have already pushed.
