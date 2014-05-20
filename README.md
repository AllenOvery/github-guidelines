github-guidelines
=================

Guidelines for using Allen &amp; Overy GitHub repositories.

## Install Git

## Local Repo
To use this repository create a folder called github-guidelines.  Navigate to your newly created folder via a bash terminal and execute the following git commands. 

```
$ cd github-guidelines
$ git init
$ git status
````

>Note that while you are grasping GitHub concepts, you should continually execute the `$ git status` command to understand the state of you local repo.

##Connect to the Remote Repository
// todo: Proxy

###From DEV

As a pre-requisite to connecting to a remote repo, ensure that you execute the following command in bash:

````
$ export https_proxy={fully qualified domain name}:{port}
````

To connect to a remote private repo from DEV, ensure that you have carried out the pre-requisites above.

````
$ git remote add origin https://{username}@github.com/allenovery/github-guidelines.git
````
Ensure that you are connected to the correct remote repo:
````
$ git remote -v
````
Now, pull from the master branch of the remote repo:
````
$ git pull origin master
````

###Outside of DEV
