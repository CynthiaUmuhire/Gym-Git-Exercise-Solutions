# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1
``` bash
umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (master)
$ git init 
Reinitialized existing Git repository in C:/Users/umuhi/Desktop/Gym-Git-Exercise-Solutions/.git/

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (master)
$ git branch -M master main 

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ touch file1.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ touch file2.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ touch file3.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ echo "helloooo">file1.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ mv file2.txt new_file2.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git remote add origin https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
error: remote origin already exists.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git remote set-url origin https://github.co
m/CynthiaUmuhire/bunde-1-exercise-1.git      

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 634 bytes | 634.00 KiB/s, done.
Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
 * [new branch]      main -> main

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git add .

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'The created files'
[main 064144b] The created files
 3 files changed, 1 insertion(+)
 create mode 100644 file1.txt
 create mode 100644 file3.txt
 create mode 100644 new_file2.txt

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (2/2), done.       
Writing objects: 100% (4/4), 353 bytes | 353.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
   a9b4ebf..064144b  main -> main

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git branch dev

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git checkout dev
Switched to branch 'dev'

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git branch test

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev       

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/CynthiaUmuhire/bunde-1-exercise-1/pull/new/dev
remote:
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was 064144b).

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git push
Everything up-to-date

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'. 

nothing to commit, working tree clean        

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$
```
### Exercise 2

```bash
umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'. 

nothing to commit, working tree clean        

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add home.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'. 

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash 
Saved working directory and index state WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add about.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'. 

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 064144b The created files
stash@{1}: WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add team.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'. 

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 064144b The created files
stash@{1}: WIP on dev: 064144b The created files
stash@{2}: WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'. 

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (5b369c17674dac8214fd5e447d92a6c5a0f8948a)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{2}
fatal: log for 'stash' only has 2 entries

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 064144b The created files
stash@{1}: WIP on dev: 064144b The created files

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'. 

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (7a659b79a67dc6ca82ad105962d191e3a92dc483)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git commit -m 'The restored files: home.html and about.html'
[dev 46efe54] The restored files: home.html and about.html
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (4/4), done.       
Writing objects: 100% (4/4), 651 bytes | 108.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
   064144b..46efe54  dev -> dev

-Solutions (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

Dropped stash@{0} (a3d8f4ac7d0e3911afee6430dd8181ecdff46538)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git reset --hard
HEAD is now at fce3544 modified home

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$
```


## Bundle 2

### Exercise 1
```bash
umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git branch ft/bundle-2

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add services.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m 'The service page'
[ft/bundle-2 af7049c] The service page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (6/6), done.       
Writing objects: 100% (6/6), 824 bytes | 206.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/CynthiaUmuhire/bunde-1-exercise-1/pull/new/ft/bundle-2    
remote:
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/bundle-2)
$
```
### Exercise 2

```bash
umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git add service.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git commit -m 'Some of our services'
[ft/service-redesign 754bab8] Some of our services
 1 file changed, 17 insertions(+)
 create mode 100644 service.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (3/3), done.       
Writing objects: 100% (3/3), 522 bytes | 522.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/CynthiaUmuhire/bunde-1-exercise-1/pull/new/ft/service-redesign
remote:
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 4, done.        
remote: Counting objects: 100% (4/4), done.  
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 709 bytes | 78.00 KiB/s, done.
From https://github.com/CynthiaUmuhire/bunde-1-exercise-1
   152e532..ec9f476  main       -> origin/main
Updating 152e532..ec9f476
Fast-forward
 service.html | 17 +++++++++++++++++
 1 file changed, 17 insertions(+)
 create mode 100644 service.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git add --all

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html
        new file:   team.html


umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git commit m 'some more services'
error: pathspec 'm' did not match any file(s) known to git
error: pathspec 'some more services' did not match any file(s) known to git

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git push
Everything up-to-date

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'some more services'
[main 9a898b2] some more services
 2 files changed, 13 insertions(+)
 create mode 100644 team.html

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (4/4), done.       
Writing objects: 100% (4/4), 575 bytes | 191.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
   ec9f476..9a898b2  main -> main

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git add --all

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git commit -m 'more services'
[ft/service-redesign 3241be7] more services
 1 file changed, 1 insertion(+)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (3/3), done.       
Writing objects: 100% (3/3), 327 bytes | 109.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
   754bab8..3241be7  ft/service-redesign -> ft/service-redesign

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git add --all

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'more services'
[main d24d688] more services
 1 file changed, 1 insertion(+)

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads      
Compressing objects: 100% (3/3), done.       
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/CynthiaUmuhire/bunde-1-exercise-1.git
   9a898b2..d24d688  main -> main

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git diff ft/service-redesign main
diff --git a/about.html b/about.html
new file mode 100644
index 0000000..9aeed59
--- /dev/null
+++ b/about.html
@@ -0,0 +1,11 @@
+<!DOCTYPE html>
+<html lang="en">
+    <head>
+        <meta charset="UTF-8">
+        <title>About page</title>
+        <meta name="viewport" content="width=device-width, initial-scale=1.0">  
+    </head>
+    <body>
+        <h1> ALL ABOUT OUR SERVISESS</h1>   
+    </body>
+</html>
\ No newline at end of file
diff --git a/home.html b/home.html
new file mode 100644
index 0000000..7f4264d
--- /dev/null

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

umuhi@IKYK MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git merge ft/service-redesign
Auto-merging service.html
Merge made by the 'ort' strategy.
 service.html | 1 +
 1 file changed, 1 insertion(+)
```

