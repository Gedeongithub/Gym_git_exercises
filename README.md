# Git exercise

## Bundle 4

### Exercise 1

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (merge)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page      
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  master
* merge

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (merge)
$ git checkout master
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (merge)
$ git diff
diff --git a/README.md b/README.md
index 574fc3e..f0eff0e 100644
--- a/README.md
+++ b/README.md
@@ -199,7 +199,7 @@ remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
 remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/home-page-redesign
 remote:
 To https://github.com/Gedeongithub/Gym_git_exercises.git
- * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
+ * [new branch] ft/home-page-redesign -> ft/home-page-redesign

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (merge)
$ git stash
Saved working directory and index state WIP on merge: 8c47c0b feat: Added menus on the homepage

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (merge)
$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git remote add origin https://github.com/Gedeongithub/git-copy.git
error: remote origin already exists.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git remote add origin https://github.com/Gedeongithub/git-copy.git
error: remote origin already exists.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git remote add git-copy https://github.com/Gedeongithub/git-copy.git

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git remote
git-copy
origin

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git add home.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   home.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git commit -m"feat: Added a new picture"
[master d0b61c8] feat: Added a new picture
 1 file changed, 1 insertion(+)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 368 bytes | 368.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Gedeongithub/Gym_git_exercises.git
   e95149b..d0b61c8  master -> master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git push git-copy
Enumerating objects: 31, done.
Counting objects: 100% (31/31), done.
Delta compression using up to 4 threads
Compressing objects: 100% (28/28), done.
Writing objects: 100% (31/31), 6.98 KiB | 476.00 KiB/s, done.
Total 31 (delta 14), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (14/14), done.
To https://github.com/Gedeongithub/git-copy.git
 * [new branch]      master -> master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$
```
