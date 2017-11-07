# Day 36

I want to display only the commits of a person:

git log --author = "John Smith"

I can also make an alias to show only my commits:

mylog =! git log --author = `git config --get user.email`

The exclamation point requires direct execution by bash.
