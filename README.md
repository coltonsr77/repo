# repo
A repo for cydia.
#### 1. Your repo is _almost_ ready.
At this point your repo is basically ready to be added into Cydia.
You can also visit your repo's homepage by going to `https://username.github.io/repo/`.
It will come with 2 sample packages, 
```sh
user:~/ $ cd repo
user:~/repo $ dpkg-scanpackages -m ./debs > Packages
user:~/repo $ bzip2 Packages
```

_Windows users, see [dpkg-scanpackages-py](https://github.com/supermamon/dpkg-scanpackages-py) or [scanpkg](https://github.com/mstg/scanpkg)._