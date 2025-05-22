# Git exercise

## Bundle 3

### Exercise 2

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git add .

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git commit -m"feat: Added home page contents"
[master 7cf85c9] feat: Added home page contents
 1 file changed, 3 insertions(+)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git switch ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git log
commit 134b75ec2bc7b1c4c75e4453956845deda66032a (HEAD -> ft/home-page-redesign, origin/ft/faq-page, ft/faq-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:56:45 2025 +0200

    feat: Added faq page

commit 4f4468fd4c9020a9c31d8277132efe3b61263af7
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:46:16 2025 +0200

    feat: added faq page

commit 20810d6e7a5d673f35c2f60b429d0ca7ea45116c
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

    feat: added faq-page

commit c2811517fd85d0dff8bfe0c1f24325f14700e1a7 (origin/ft/contact-page, ft/contact-page)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    ft:added contact us

commit e95149b0dd283338281dd928768e8f20c06fec24 (origin/master)
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

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git rebase master
Successfully rebased and updated refs/heads/ft/home-page-redesign.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git log
commit ae94bc416e888bdb200d71e3195ed63c2abc1ecf (HEAD -> ft/home-page-redesign)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:56:45 2025 +0200

    feat: Added faq page

commit 3c85b14e3da7eaa372b0f9830da153f8859d101d
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:46:16 2025 +0200

    feat: added faq page

commit 1cee1b8f8ee2dbeac52df17ed7fcdf41408539f6
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:24:14 2025 +0200

    feat: added faq-page

commit 34c05463b30cdd290ce32589f7505229b4aec14a
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Wed May 21 17:09:00 2025 +0200

    ft:added contact us

commit 7cf85c97690644be32aceb9c08ff99400a571dac (master)
Author: Gedeon DUFITIMANA <gedeon.dufitimana2023@kepler.org>
Date:   Thu May 22 10:35:50 2025 +0200

    feat: Added home page contents


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git add home.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git commit -m"feat: Added menus on the homepage"
[ft/home-page-redesign 4b477a9] feat: Added menus on the homepage
 1 file changed, 5 insertions(+)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 23, done.
Counting objects: 100% (23/23), done.
Delta compression using up to 4 threads
Compressing objects: 100% (19/19), done.
Writing objects: 100% (19/19), 5.04 KiB | 224.00 KiB/s, done.
Total 19 (delta 10), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (10/10), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/home-page-redesign)
$
```
