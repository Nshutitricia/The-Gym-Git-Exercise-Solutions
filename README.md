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

```