# pyGit
pyGit is a automatic git helper, written in python, using the gitpython library.

When run, it will look through the given repos, fetch and check for updates, pull if needed. 

Then look local after untracted files and dirty files, add these and commit for push.

A prompt is given, when a commit msg is needed. 

I choose to keep track of the commits by having a manual input message.

This can be changed, if wanted.


## How to install!

#### gitpy_ssh
first need to tell where the ssh key is located. Alter the address field and write the location of the id_rsa file.

#### repos.cfg
Here all the repos with remote address, using SSH and local path is set.

How many repos, is up to you. 

#### user.cfg
ssh = Set the address for the given gitpy_ssh file, if not changed it will be in the folder together with the application

name = This is your git username

email = git email address

#### pygit

On line 75, insert the full path to the user.cfg file

On line 92, insert the full path to the repos.cfg file









### Symlinks
Last step of installation, is adding a symlink to [path].

```
sudo ln -s /home/location/pygit.py /usr/local/bin/pygit
```

Then the command pygit can be used to run the app from your terminal
