# Git exercise

## Bundle 3

### Exercise 1

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git add team.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git commit -m"added team page"
[ft/team-page 3df7f7e] added team page
 1 file changed, 1 insertion(+), 1 deletion(-)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 306 bytes | 306.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Gedeongithub/Gym_git_exercises.git
   92ce250..3df7f7e  ft/team-page -> ft/team-page

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git checkout master
M       README.md
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git checkout -b ft/contact-page
fatal: a branch named 'ft/contact-page' already exists

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git checkout ft/team-page
M       README.md
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git log
commit 3df7f7e7edfbdc81f34b418881e389d8c9150b44 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    added team page

commit 92ce250cb8609dbee6b0d6cd7778982eea109d85
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 12:08:20 2025 +0200


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git checkout ft/contact-page
M       README.md
Switched to branch 'ft/contact-page'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page)
$ git cherry-pick 3df7f7e7edfbdc81f34b418881e389d8c9150b44
CONFLICT (modify/delete): team.html deleted in HEAD and modified in 3df7f7e (added team page).  Version 3df7f7e (added team page) of team.html left in tree.
error: could not apply 3df7f7e... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
hint: Disable this message with "git config advice.mergeConflict false"

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git touch contact.html
git: 'touch' is not a git command. See 'git --help'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ touch contact.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git add --all

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 3df7f7e.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        modified:   README.md
        new file:   contact.html
        new file:   team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git reset HEAD README.md
Unstaged changes after reset:
M       README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 3df7f7e.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        new file:   contact.html
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page|CHERRY-PICKING)
$ git commit -m"ft:added contact us"
[ft/contact-page c281151] ft:added contact us
 Date: Wed May 21 17:09:00 2025 +0200
 2 files changed, 22 insertions(+)
 create mode 100644 contact.html
 create mode 100644 team.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page)
$  git push --set-upstream origin ft/contact-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 555 bytes | 555.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/contact-page
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/contact-page)
$ git checkout -b ft/fag-page
Switched to a new branch 'ft/fag-page'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/fag-page)
$ git branch -M ft/fag-page ft/faq-page

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ touch faq.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git add --all

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   faq.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git reset HEAD README.md
Unstaged changes after reset:
M       README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git commit -m"feat: added faq-page"
[ft/faq-page 20810d6] feat: added faq-page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/faq-page
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git log
commit 20810d6e7a5d673f35c2f60b429d0ca7ea45116c (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

    feat: added faq-page

commit c2811517fd85d0dff8bfe0c1f24325f14700e1a7 (origin/ft/contact-page, ft/contact-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    ft:added contact us

commit e95149b0dd283338281dd928768e8f20c06fec24 (origin/master, master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 11:05:58 2025 +0200

    ft: Added old services

commit fca26f55b0b136bce9f8b7f0dbc3b6755b177f43
Merge: 4f56495 5e3f8e6
Author: Gedeon DUFITIMANA <123157177+Gedeongithub@users.noreply.github.com>
Date:   Wed May 21 10:05:21 2025 +0200

    Merge pull request #3 from Gedeongithub/ft/bundle-2

    Add a new html page to a project

commit 4f564950d9325483a4891fac62979a8ac8fddefc
Merge: 547ff54 9756f56
Author: Gedeon DUFITIMANA <123157177+Gedeongithub@users.noreply.github.com>
Date:   Wed May 21 10:04:55 2025 +0200

    Merge pull request #2 from Gedeongithub/dev

    The setup of home and about page

commit 5e3f8e668b0f875e460aa4213bf88b70f6eaa139 (origin/ft/bundle-2, ft/bundle-2)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Sat May 17 14:47:30 2025 +0200

    create a services page

commit 9756f5600d0a8d8b7ebb416d1609f9b06e655085 (dev)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Sat May 17 13:03:00 2025 +0200

    The setup of home and about page

commit 547ff543002195677b131d824d4c2784f75a2d3f
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 14:32:34 2025 +0200

    added the creation of dev and test as well as deleting both test locally and remotely

commit 08eb80208794fa1ca5e53ca6aba2e8e03a23b5c2
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 12:16:27 2025 +0200

    first commit

commit 3ed949db5733019b4c1c63365869f8bdf57a5626
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 12:14:18 2025 +0200

    my initial git

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git switch ft/team-page
M       README.md
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git log
commit 3df7f7e7edfbdc81f34b418881e389d8c9150b44 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    added team page

commit 92ce250cb8609dbee6b0d6cd7778982eea109d85
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 12:08:20 2025 +0200

    added team page

commit e95149b0dd283338281dd928768e8f20c06fec24 (origin/master, master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 11:05:58 2025 +0200

    ft: Added old services

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/team-page)
$ git switch ft/faq-page
M       README.md
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git log
commit 20810d6e7a5d673f35c2f60b429d0ca7ea45116c (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

    feat: added faq-page

commit c2811517fd85d0dff8bfe0c1f24325f14700e1a7 (origin/ft/contact-page, ft/contact-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git revert 3df7f7e7edfbdc81f34b418881e389d8c9150b44
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...
Vim: Finished.
error: there was a problem with the editor 'vi'
Please supply the message using either -m or -F option.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git revert 3df7f7e7edfbdc81f34b418881e389d8c9150b44
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git log
commit 20810d6e7a5d673f35c2f60b429d0ca7ea45116c (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

    feat: added faq-page

commit c2811517fd85d0dff8bfe0c1f24325f14700e1a7 (origin/ft/contact-page, ft/contact-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    ft:added contact us

commit e95149b0dd283338281dd928768e8f20c06fec24 (origin/master, master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 11:05:58 2025 +0200

    ft: Added old services

commit fca26f55b0b136bce9f8b7f0dbc3b6755b177f43
Merge: 4f56495 5e3f8e6
Author: Gedeon DUFITIMANA <123157177+Gedeongithub@users.noreply.github.com>
Date:   Wed May 21 10:05:21 2025 +0200

    Merge pull request #3 from Gedeongithub/ft/bundle-2

    Add a new html page to a project

commit 4f564950d9325483a4891fac62979a8ac8fddefc
Merge: 547ff54 9756f56
Author: Gedeon DUFITIMANA <123157177+Gedeongithub@users.noreply.github.com>
Date:   Wed May 21 10:04:55 2025 +0200

    Merge pull request #2 from Gedeongithub/dev

    The setup of home and about page

commit 5e3f8e668b0f875e460aa4213bf88b70f6eaa139 (origin/ft/bundle-2, ft/bundle-2)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Sat May 17 14:47:30 2025 +0200

    create a services page

commit 9756f5600d0a8d8b7ebb416d1609f9b06e655085 (dev)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Sat May 17 13:03:00 2025 +0200

    The setup of home and about page

commit 547ff543002195677b131d824d4c2784f75a2d3f
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 14:32:34 2025 +0200

    added the creation of dev and test as well as deleting both test locally and remotely

commit 08eb80208794fa1ca5e53ca6aba2e8e03a23b5c2
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 12:16:27 2025 +0200

    first commit

commit 3ed949db5733019b4c1c63365869f8bdf57a5626
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 15 12:14:18 2025 +0200

    my initial git

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git commit -m"feat: added faq page"
[ft/faq-page 4f4468f] feat: added faq page
 1 file changed, 1 insertion(+), 1 deletion(-)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git log
commit 4f4468fd4c9020a9c31d8277132efe3b61263af7 (HEAD -> ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:46:16 2025 +0200

    feat: added faq page

commit 20810d6e7a5d673f35c2f60b429d0ca7ea45116c (origin/ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

:
```
