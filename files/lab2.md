# LAB 2

## Adding (Modifying repository), Staging and Committing files. Checking logs and deleting files.  

Read through commands then practice with hands on exercises.

**git status** - current repository status
```
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
```

Adding a file to repository

```
$ ls > files-ds.txt
```

**git status** - current repository status (Modified)
```
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        files-ds.txt

nothing added to commit but untracked files present (use "git add" to track)
```
**git-add** - Add files to "Staging" area

```
$ git add files-ds.txt
warning: LF will be replaced by CRLF in files-ds.txt.
The file will have its original line endings in your working directory.
```

**git-commit** - Commit file to repository
```
$ git commit -m "Added files-ds.txt"
[master f46d0d4] Added files-ds.txt
 1 file changed, 4 insertions(+)
 create mode 100644 files-ds.txt
```

**git-push** - Push modifications to remote repository
```
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 376 bytes | 188.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.jci.com/jsikard/git-workshop.git
   3664d3d..f46d0d4  master -> master
```

Adding, staging, commiting and pushing. Hands on practice. 

1.  Change directory to git-workshop if not there already
```
$ cd git-workshop
```
2. Add a file (Modify repository)
```
$ ls > files-<your-initials>.txt
```
3. Add to Staging area
```
$ git add files-<your-initials>.txt
```
4. Commit 
```
$ git commit -m "Added files-<your-initials>.txt"
```
5. Push to remote repository 
```
$ git push
```
6. For good measure, check last 5 log entries (-5 switch)
```
$ git log -5
```

[Go to Lab 3](lab3.md)
