# Day 4

I want to change my last commit, because I put a bad
commit message.

    git commit --amend

Modifies the last commit message. Can also add the changes to your staging area.

    git add myfile.erl && git commit --amend

Adds the modification of myfile.erl to the previous commit.

This command rewrites the git history; DO NOT do it if you have already pushed.
