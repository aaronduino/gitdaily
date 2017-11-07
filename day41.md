# Day 41

I want to group two git repositories into one:

    git replace SHA1 SHA2

The SHA1 commit will be replaced by SHA2 and all of its parents.

I've never used this command other than to test it, but
it can be useful if you have a large history and do not need to keep it completely.

That's what was done for the otp repository that is over 300 MB: https://github.com/erlang/otp/wiki/Extending-the-history-of-Erlang-OTP.

You can easily test it with a few commands to link two repositories. Link the EventMachine and NodeJS repositories.

    $ git clone https://github.com/eventmachine/eventmachine.git
    $ git remote add nodejs https://github.com/joyent/node.git
    $ git fetch nodejs
    $ git replace d9a23e4779b3f555e63e4ff565ef0848a8bcabd4 61dfe5d2a9f613e3826997efa189ec8dd239aacf

Yes it is useless. But look at the git log and everything happens as if nothing had happened.

`git help replace` (but it will not help you much)

http://progit.org/2010/03/17/replace.html
