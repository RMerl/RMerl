## Migration of project repos to a new Github Organization account

The Asuswrt-Merlin related repos have been migrated to a new organization account named [@asuswrt-merlin](https://github.com/asuswrt-merlin).

While existing links pointing here will be forwarded automatically, it is strongly recommended that you update your existing links, and cloned repos to use the new remote.  Example here to move the main asuswrt-merlin.ng remote to the new location:

```
merlin@ubuntu-dev2:~/dev/amng$ git remote -v
origin	git@github.com:RMerl/asuswrt-merlin.ng.git (fetch)
origin	git@github.com:RMerl/asuswrt-merlin.ng.git (push)
merlin@ubuntu-dev2:~/dev/amng$ git remote set-url origin git@github.com:Asuswrt-Merlin/asuswrt-merlin.ng.git
merlin@ubuntu-dev2:~/dev/amng$ git remote -v
origin	git@github.com:Asuswrt-Merlin/asuswrt-merlin.ng.git (fetch)
origin	git@github.com:Asuswrt-Merlin/asuswrt-merlin.ng.git (push)
```

If you are using https instead of SSH to clone the repo, then use the appropriate URL instead - just replacing "RMerl" with "Asuswrt-Merlin".

Repeat this for any repo that you were cloning (asuswrt-merlin.ng, am-toolchains, etc...)

More information here: https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories
