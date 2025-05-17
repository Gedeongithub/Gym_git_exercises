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
