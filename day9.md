# Day 9

I want to know all the commits since yesterday.

git log --since yesterday

A small bonus today:

git log HEAD ^

Lists the commits from the penultimate commit.

git log HEAD ~ 4 ..

List the last four commit. Equivalent to :

git log HEAD ~ 4..HEAD

More informations:

git help revisions
