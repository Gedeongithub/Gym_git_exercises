# Git exercise

## Bundle 4

### Exercise 2

```bash
Exercise Solutions (master)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ touch footer.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ gits status
bash: gits: command not found

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        footer.html

nothing added to commit but untracked files present (use "git add" to track)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git add footer.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   footer.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git commit -m"Added footer file"
[ft/footer b2768dc] Added footer file
 1 file changed, 11 insertions(+)
 create mode 100644 footer.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
nothing to commit, working tree clean

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git add --all

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   footer.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git commit -m"Added footer content"
[ft/footer a92f84b] Added footer content
 1 file changed, 6 insertions(+), 1 deletion(-)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 2.18 KiB | 372.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), done.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/footer
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

nothing to commit, working tree clean

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git merge --squash ft/footer
Updating e5722a3..a92f84b
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 footer.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git log
commit e5722a317f455c805c200d89932ac0b10bb4c4e2 (HEAD -> ft/squashing, git-copy/master, master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 22 15:38:46 2025 +0200

    feat: Added a new picture

commit d0b61c800f755e519bc85e45021912b3b89ac846 (origin/master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 22 15:29:58 2025 +0200


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git lg
git: 'lg' is not a git command. See 'git --help'.

The most similar command is
        log

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git commit -m"footer change squashing"
[ft/squashing e1ddc6a] footer change squashing
 1 file changed, 16 insertions(+)
 create mode 100644 footer.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git log
commit e1ddc6a98d0281a9d4270a7d6436db0f887ff146 (HEAD -> ft/squashing)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Fri May 23 10:42:59 2025 +0200

    footer change squashing

commit e5722a317f455c805c200d89932ac0b10bb4c4e2 (git-copy/master, master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 22 15:38:46 2025 +0200


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/footer
  ft/home-page-redesign
  ft/service-redesign
* ft/squashing
  ft/team-page
  master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git checkout ft/footer
Switched to branch 'ft/footer'
Your branch is up to date with 'origin/ft/footer'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git log
commit a92f84b66534c2dc6a2cd7150015d986cdd1a9de (HEAD -> ft/footer, origin/ft/footer)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Fri May 23 10:05:23 2025 +0200

    Added footer content

commit b2768dcc2cee65c8be76194153d02f54f27f961a
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Fri May 23 10:01:59 2025 +0200


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/footer)
$ git checkout ft/squashing
Switched to branch 'ft/squashing'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git push
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git push --set-upstream origin ft/squashin
error: src refspec ft/squashin does not match any
error: failed to push some refs to 'https://github.com/Gedeongithub/Gym_git_exercises.git'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$ git push --set-upstream origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 494 bytes | 164.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/squashing
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/squashing)
$
```
