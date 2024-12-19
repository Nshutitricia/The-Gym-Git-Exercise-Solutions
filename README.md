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

 ## Exercise 2

 ```bash
gymisaro@Isaros-iMac Git-solutions % git checkout master
Switched to branch 'master'
gymisaro@Isaros-iMac Git-solutions % git pull origin master
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 889 bytes | 444.00 KiB/s, done.
From https://github.com/Nshutitricia/Git-solutions
 * branch            master     -> FETCH_HEAD
   2948337..e7d1858  master     -> origin/master
Updating 2948337..e7d1858
Fast-forward
 services.html | 11 +++++++++++
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

 gymisaro@Isaros-iMac Git-solutions % git checkout -b ft/service-
redesign
Switched to a new branch 'ft/service-redesign'
gymisaro@Isaros-iMac Git-solutions % git commit -a -m "service f
ile changes"
[ft/service-redesign b9ae6a0] service file changes
 1 file changed, 1 insertion(+)
gymisaro@Isaros-iMac Git-solutions % git push origin ft/service-
redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 350 bytes | 350.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Nshutitricia/Git-solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/Nshutitricia/Git-solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

 gymisaro@Isaros-iMac Git-solutions % git checkout master
Switched to branch 'master'
gymisaro@Isaros-iMac Git-solutions % git commit -a -m  "Made som
e changes to services"
[master d591267] Made some changes to services
 1 file changed, 2 insertions(+), 1 deletion(-)
gymisaro@Isaros-iMac Git-solutions % git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 360 bytes | 360.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nshutitricia/Git-solutions.git
   e7d1858..d591267  master -> master
gymisaro@Isaros-iMac Git-solutions % git checkout ft/service-red
esign
Switched to branch 'ft/service-redesign'
gymisaro@Isaros-iMac Git-solutions % git diff origin/master
diff --git a/services.html b/services.html
index 253a16b..1fccf7e 100644
--- a/services.html
+++ b/services.html
@@ -6,7 +6,7 @@
     <title>Document</title>
 </head>
 <body>
-    <h1>This are my services no way</h1>
-    <p>I am now in the branch of master</p>
+    <h1>This are my services</h1>
+    <p>I just created a new branch of services</p>
 </body>
 </html>
\ No newline at end of file
gymisaro@Isaros-iMac Git-solutions % git checkout master
Switched to branch 'master'
gymisaro@Isaros-iMac Git-solutions % git merge ft/service-redesi
gn
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
gymisaro@Isaros-iMac Git-solutions % git commit -m "Merged"
[master 86c743e] Merged
gymisaro@Isaros-iMac Git-solutions % git push origin master
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 370 bytes | 370.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nshutitricia/Git-solutions.git
   d591267..86c743e  master -> master
 ```