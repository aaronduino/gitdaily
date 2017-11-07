# Day 30

I want my bash to show in which branch I am. In ~ / .bashrc,
I add at the end of the file:

PS1 = '\ w $ (__ git_ps1) \ $'

\ w indicates the current directory,
$ (_ \ _ git \ _ps1) is your branch
and \ $ prints # if you are superuser.
