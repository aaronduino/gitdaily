# Day 40

You have recurring conflicts during the merge and you want to correct them once and for all.

The first thing to do is to configure the variable *rerere.enabled*.

    git config --global rerere.enabled 1

Then? You let go git. It will automatically record conflicts and their resolutions to repeat the same thing automatically.

The next git pull --rebase or git merge, no need to reapply the same fix.

If you have recorded a bad resolution, you can use git rerere forget.

And why rerere? This is the abbreviation of Reuse recorded resolution.

    git help rerere

http://progit.org/2010/03/08/rerere.html
