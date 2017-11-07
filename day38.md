# Day 38

I want to create a git repository from another repository to keep some of the history.

For example to create a git repository of the lib/captcha subdirectory.

    git filter-branch --subdirectory-filter / captcha - --all

filter-branch will replace your current git repository by keeping only the files and commits corresponding to lib/captcha.
lib/captcha will become the current directory.

You can also delete a file from your git history.

        git filter-branch --index-filter 'git rm --cached --ignore-unmatch config/prod.yml' HEAD

Rewrite all commits so that the config/prod.yml file is not there anymore.

    git help filter-branch

To test these commands, use a new clone of your favorite project. Or wait for the latest Git "Hardcore" Daily.
