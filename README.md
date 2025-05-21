# Git exercise

## Bundle 1

### Exercise 1

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git log
fatal: your current branch 'main' does not have any commits yet

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git branch

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git remote
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git remote
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git remote

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git stash
You do not have the initial commit yet

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (main)
$ git branch -m main master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git checkout -b dev
Switched to a new branch 'dev'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
nothing to commit, working tree clean

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git add .

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
nothing to commit, working tree clean

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/dev
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git push
Everything up-to-date

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git checkout -b test
Switched to a new branch 'test'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git push
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin test

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git push --set- upstream origin test
error: src refspec origin does not match any
error: failed to push some refs to 'upstream'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git add -all
error: did you mean `--all` (with two dashes)?

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git add -All
error: unknown switch `l'
usage: git add [<options>] [--] <pathspec>...

    -n, --[no-]dry-run    dry run
    -v, --[no-]verbose    be verbose

    -i, --[no-]interactive
                          interactive picking
    -p, --[no-]patch      select hunks interactively
    -e, --[no-]edit       edit current diff and apply
    -f, --[no-]force      allow adding otherwise ignored files
    -u, --[no-]update     update tracked files
    --[no-]renormalize    renormalize EOL of tracked files (implies -u)
    -N, --[no-]intent-to-add
                          record only the fact that the path will be added later
    -A, --[no-]all        add changes from all tracked and untracked files
    --[no-]ignore-removal ignore paths removed in the working tree (same as --no-all)
    --[no-]refresh        don't add, only refresh the index
    --[no-]ignore-errors  just skip files which cannot be added because of errors
    --[no-]ignore-missing check if - even missing - files are ignored in dry run
    --[no-]sparse         allow updating entries outside of the sparse-checkout cone
    --[no-]chmod (+|-)x   override the executable bit of the listed files
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git add .

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git status
On branch test
nothing to commit, working tree clean

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git push
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin test

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git push --set-upstream origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/test
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (test)
$ git switch dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git branch -D test
Deleted branch test (was 08eb802).

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git push --origin delete test
error: unknown option `origin'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --[no-]verbose    be more verbose
    -q, --[no-]quiet      be more quiet
    --[no-]repo <repository>
                          repository
    --[no-]all            push all branches
    --[no-]branches       alias of --all
    --[no-]mirror         mirror all refs
    -d, --[no-]delete     delete refs
    --[no-]tags           push tags (can't be used with --all or --branches or --mirror)
    -n, --[no-]dry-run    dry run
    --[no-]porcelain      machine-readable output
    -f, --[no-]force      force updates
    --[no-]force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --[no-]force-if-includes
                          require remote updates to be integrated locally
    --[no-]recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --[no-]thin           use thin pack
    --[no-]receive-pack <receive-pack>
                          receive pack program
    --[no-]exec <receive-pack>
                          receive pack program
    -u, --[no-]set-upstream
                          set upstream for git pull/status
    --[no-]progress       force progress reporting
    --[no-]prune          prune locally removed refs
    --no-verify           bypass pre-push hook
    --verify              opposite of --no-verify
    --[no-]follow-tags    push missing but relevant tags
    --[no-]signed[=(yes|no|if-asked)]
                          GPG sign the push
    --[no-]atomic         request atomic transaction on remote side
    -o, --[no-]push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git push origin --delete test
To https://github.com/Gedeongithub/Gym_git_exercises.git
 - [deleted]         test

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$
```
### Exercise 2

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ touch home.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash
No local changes to save

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash list

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ ls
home.html  README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git add home.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ ls
README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ touch about.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ ls
about.html  README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git add about.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 08eb802 first commit
stash@{1}: WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ touch team.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git add team.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 08eb802 first commit
stash@{1}: WIP on dev: 08eb802 first commit
stash@{2}: WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (db2e9d13bf936d29391c7919ccf7868ee6cdbf1e)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 08eb802 first commit
stash@{1}: WIP on dev: 08eb802 first commit

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (e53b06c9cb2386a775539e9f6dd24d4d8b06b2c3)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$ ls
about.html  home.html  README.md

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (dev)
$
```
## Bundle 2
### Exercise 2

```bash
Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/bundle-2)
$ git branch
  dev
* ft/bundle-2
  master

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/bundle-2)
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git pull
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (6/6), 3.41 KiB | 174.00 KiB/s, done.
From https://github.com/Gedeongithub/Gym_git_exercises
   547ff54..fca26f5  master     -> origin/master
   9756f56..51b8c4c  dev        -> origin/dev
Updating 547ff54..fca26f5
Fast-forward
 README.md    | 165 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html   |  11 ++++
 home.html    |  12 +++++
 service.html |  11 ++++
 4 files changed, 199 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 service.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (master)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

no changes added to commit (use "git add" and/or "git commit -a")

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git add .

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html
        new file:   team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git reset HEAD team.html

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git add service.html 

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m"ft: Added the list of the new service"
[ft/service-redesign b87e774] ft: Added the list of the new service
 1 file changed, 7 insertions(+), 1 deletion(-)

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 504 bytes | 504.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Gedeongithub/Gym_git_exercises/pull/new/ft/service-redesign
remote:
To https://github.com/Gedeongithub/Gym_git_exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

Administrator@DESKTOP-5O3LLQR MINGW64 /e/Gym Git Exercise Solutions (ft/service-redesign)
$
```
