# Reposi3
A Cydia repository template. This template contains sample on how you can easily make depiction pages without replicating your html pages. The pages are styled using [Bootsrap](http://getbootstrap.com/) which is really easy to use. You can see how it looks like by visiting [this sample repo](https://supermamon.github.io/Reposi3/) on your desktop or mobile phone.

Most data for this repo is stored on XML files and are loaded on the depiction page dynamically. See the guide below on how to set it up. Note that this guide doesn't cover creating .deb files but will briefly cover assiging depictions.

## How to use this template

### 1. Download

If you are *not* hosting your repo on [Github Pages](https://pages.github.com/), you can download the zip file [here](https://github.com/supermamon/Reposi3/archive/master.zip) and extract to a subfolder on your website.

There are 2 options for those using [Github Pages](https://pages.github.com/).

A. If you want to use your root `username.github.io` as your repo, fork this repo and rename it to `username.github.io`. So when adding it in Cydia, use `https://username.github.io`.

B. If you want to use a subfolder for your existing `username.github.io` as your repo (example `username.github.io/repo`), fork this repo and rename it to `repo`. So when adding it in Cydia, use `https://username.github.io/repo`.

You can change `repo` to anything you want, like 
#### 3. Your repo is _almost_ ready.
At this point your repo is basically ready to be added into Cydia.
You can also visit your repo's homepage by going to `https://username.github.io/repo/`.
It will come with 2 sample packages, 
```sh
user:~/ $ cd repo
user:~/repo $ dpkg-scanpackages -m ./debs > Packages
user:~/repo $ bzip2 Packages
```

_Windows users, see [dpkg-scanpackages-py](https://github.com/supermamon/dpkg-scanpackages-py) or [scanpkg](https://github.com/mstg/scanpkg)._

#### 5. Cydia at last!

If you haven't done yet, go ahead and add your repo to Cydia.
You should now be able to install your tweak into your own repo.

### Cleanup

Just a cleanup step, remove the debs that came with this template and re-run the commands on step 3. You can keep the sample depictions for reference by they're not needed for your repo.