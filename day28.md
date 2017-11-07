# Day 28

You want to look for the commit that introduced a regression.

    git bisect start

Will start a bug search session. Bisect will place you on
specific commits, and you'll have to mark them good or bad for
finally find the corresponding commit.

    git help bisect
