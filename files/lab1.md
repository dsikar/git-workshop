# LAB 1

1. Open Git-Bash and change directory to ~/Documents
```
$ cd ~/Documents
```
2. Create jci-git directory
```
$ mkdir jci-git
```
3. Change directory to jci-git
```
$ cd jci-git
```
4. Configure your email address and user name 
```
$ git config --global user.email JCIGlobalID@jci.com - note use your own JCI email address, name in quotes 
$ git config --global user.name "My Name"
```
5. Check configuration
```
$ git config --global user.email
$ git config --global user.name
```
6.  Clone a repository - note you might have to append your JCI Global ID to URL like such https://jsikard@github.jci.com/jsikard/git-workshop.git
```
$ git clone https://github.jci.com/jsikard/git-workshop.git
Cloning into 'git-workshop'...
remote: Counting objects: 39, done.
remote: Compressing objects: 100% (35/35), done.
remote: Total 39 (delta 9), reused 18 (delta 3), pack-reused 0
Unpacking objects: 100% (39/39), done.
```
7. Change directory to git-workshop
```
$ cd git-workshop
```
8. Inspect files
```
$ ls -last
```
9. Find out where remote repository is
```
$ git remote
origin
```
10. Use **verbose -v** switch for added information
```
$ git remote -v
origin  https://jsikard@github.jci.com/jsikard/git-workshop.git (fetch)
origin  https://jsikard@github.jci.com/jsikard/git-workshop.git (push)
```
11. Show the branches that exist in your local repository
```
$ git branch
```
12. Show branches that exist in the remote repository
```
$ git branch -v
```

[Go to Lab 2](lab2.md)
