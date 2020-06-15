# Test Repo for [git-crypt](https://github.com/CyberScout/git-crypt)

This is a tiny repo that contains some plaintext and some encrypted
files. Check it out to test whether your `git-crypt` setup works.

There is a file called `secure/secrets.txt`. If
`git-crypt` is working, you will be able to read the contents of
this file.

> This is an encrypted file, but you can totally read it. Fancy!

The other files are in plaintext, and you should be able to read
those, too.

## GPG mode

Make sure your system is properly configured:

[GPGTools for macOS](https://cyberscout.atlassian.net/wiki/spaces/AD/pages/374079530/GPGTools+for+macOS)
|
[GnuPG for Windows](https://cyberscout.atlassian.net/wiki/spaces/AD/pages/376733742/GnuPG+for+Windows)

[git-crypt](https://cyberscout.atlassian.net/wiki/spaces/AD/pages/378929153/git-crypt)

You will need to follow the instructions in the above documents
to provide a key ID or fingerprint to someone with write access
on this repo.

Then, pull the changes. You should be able to

```bash
$ git crypt unlock
```

## Symmetric mode

The key is located at `./git-crypt-test.key`.

----

:warning: Normally, the key would **not** be checked into the
repository. This is a security risk, and in fact defeats he purpose
of encrypting files in the repo in the first place. This is done
here for demonstration purposes. _**DON'T DO THIS IN YOUR OWN
REPOSITORIES!!!**_ Seriously. Don't do it.

----

```bash
$ git crypt unlock ./git-crypt-test.key
```
