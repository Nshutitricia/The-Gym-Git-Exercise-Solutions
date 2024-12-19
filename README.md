# Git Exercises

## Bundle 1

## Exercise 1

```bash
gymisaro@Isaros-iMac Git-solutions % git branch
gymisaro@Isaros-iMac Git-solutions % git branch -M master
gymisaro@Isaros-iMac Git-solutions % git add .
gymisaro@Isaros-iMac Git-solutions % git commit -m "This is index"
[master (root-commit) fa0662f] This is index
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
gymisaro@Isaros-iMac Git-solutions % git branch
* master
gymisaro@Isaros-iMac TheGymGit % git remote add origin https://github.com/Nshutitricia/The-Gym-Git-Exercise-Solutions.git

gymisaro@Isaros-iMac Git-solutions % git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 374 bytes | 374.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nshutitricia/Git-solutions.git
 * [new branch]      master -> master
 gymisaro@Isaros-iMac Git-solutions % git checkout -b dev
Switched to a new branch 'dev'
gymisaro@Isaros-iMac Git-solutions % git checkout -b test
Switched to a new branch 'test'
gymisaro@Isaros-iMac Git-solutions % git checkout dev
Switched to branch 'dev'
gymisaro@Isaros-iMac Git-solutions % git branch -d test
Deleted branch test (was fa0662f).
```

## Exercise 2

```bash
gymisaro@Isaros-iMac Git-solutions % git stash pop stash@{1}
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (a10ebba247e6db02235c7cd16d4f5d4bd33d3a4f)
gymisaro@Isaros-iMac Git-solutions % git stash pop stash@{1}
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (bf040a9add53b5beb08b06d8cdc4cf2f8e24e698)

gymisaro@Isaros-iMac Git-solutions % git commit -m "This is stas
h"
[master 2948337] This is stash
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 gymisaro@Isaros-iMac Git-solutions % git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 513 bytes | 513.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Nshutitricia/Git-solutions.git
   fa0662f..2948337  master -> master
   gymisaro@Isaros-iMac Git-solutions % git stash pop stash@{0}
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (cb3f88f26f90d64502871d717be3724e6755bd1d)

gymisaro@Isaros-iMac Git-solutions % git log --oneline
2948337 (HEAD -> master, origin/master) This is stash
fa0662f (dev) This is index
'git <command> [<revision>...] -- [<file>...]'
gymisaro@Isaros-iMac Git-solutions % git reset --hard 2948337
HEAD is now at 2948337 This is stash
```

## Bundle 2

## Exercise 1

```bash

gymisaro@Isaros-iMac Git-solutions % git checkout -b ft/bundle-2

Switched to a new branch 'ft/bundle-2'
gymisaro@Isaros-iMac Git-solutions % git add .
gymisaro@Isaros-iMac Git-solutions % git commit -m "Services"  
[ft/bundle-2 69d1b08] Services
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
gymisaro@Isaros-iMac Git-solutions % git push origin ft/bundle-2

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 438 bytes | 438.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Nshutitricia/Git-solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/Nshutitricia/Git-solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
 ```