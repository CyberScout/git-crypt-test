# Test Repo for [git-crypt](https://github.com/CyberScout/git-crypt)

This is a tiny repo that contains some plaintext and some encrypted
files. Check it out to test whether your `git-crypt` setup works.

First, use the secret key that is checked into this repository to
unlock the repo with `git-crypt`.

----

:warning: Normally, the key would **not** be checked into the
repository. This is a security risk, and in fact defeats he purpose
of encrypting files in the repo in the first place. This is done
here for demonstration purposes. _**DON'T DO THIS IN YOUR OWN
REPOSITORIES!!!**_

----

This repository contains a file called `secure/secrets.txt`. If
`git-crypt` is working, you will be able to read the contents of
this file.

> This is an encrypted file, but you can totally read it. Fancy!

The other files are in plaintext, and you should be able to read
those, too.
