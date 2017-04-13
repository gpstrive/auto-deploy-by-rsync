auto-deploy-by-rsync
====================
Changes: To make the script work on mac
Notices: If you have any trouble on mac with the script, leave an issue

use inotify to check files change and auto deploy.

## Install

Copy or link `auto-deploy-by-rsync`, `mac-auto-deploy` into you $PATH. 

Just like `ln -s ~/projects/auto-deploy-by-rsync/mac-auto-deploy /usr/local/bin`.

## Linux

Before using this script, you need to do `sudo apt-get install inotify-tools`.


And run this on your project folder.

```
auto-deploy-by-rsync . user@everet.org:~/work/2959_add_new_type_awards
```


## Mac
In Mac OS X, we need fswatch and ssh with public-key.

```
brew install fswatch
```

And run this on your project folder.

```
mac-auto-deploy . gzhualiang@dev35:~/git/project
```
