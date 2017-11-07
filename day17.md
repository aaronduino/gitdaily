# Day 17

I want to add a great 'chuck' command that answers 'norris' (ahah).

$ cat> / usr / local / bin / git-chuck <<< EOF
#! / Bin / sh
echo 'norris'
EOF
$ chmod + x / usr / local / bin / git-chuck
$ git chuck

This will create an executable "git-chuck" that simply responds "norris".
git recognizes executables that are called git-xxx.
That's how it works:

* git-pulls: https://github.com/schacon/git-pulls
* git-pair: https://github.com/chrisk/git-pair

and many others.
