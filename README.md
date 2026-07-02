# git Exercises

## Bundel 1

### Exercises 1

```bash
Gym-Git-Exercise-Solutions (main) $ git init
Reinitialized existing Git repository in C:/Users/rukun/OneDrive/Desktop/The Gym/TheGym_git_exercises/Gym-Git-Exercise-Solutions/.git/
Gym-Git-Exercise-Solutions (main) $ git branch dev
Gym-Git-Exercise-Solutions (main) $ git branch test
Gym-Git-Exercise-Solutions (main) $ git status
On branch main
nothing to commit, working tree clean
Gym-Git-Exercise-Solutions (main) $ git log
commit 5f3c3ff9c932956397934eab15299de432301369 (HEAD -> main, test, dev)
Author: Bless <rukundobless47@gmail.com>
Date:   Thu Jul 2 16:16:18 2026 +0200

    Initial commit
Gym-Git-Exercise-Solutions (main) $ git brach -d test
git: 'brach' is not a git command. See 'git --help'.

The most similar command is
        branch
Gym-Git-Exercise-Solutions (main) $ git branch -d test
Deleted branch test (was 5f3c3ff).
Gym-Git-Exercise-Solutions (main) $ git log
commit 5f3c3ff9c932956397934eab15299de432301369 (HEAD -> main, dev)
Author: Bless <rukundobless47@gmail.com>
Date:   Thu Jul 2 16:16:18 2026 +0200

    Initial commit
Gym-Git-Exercise-Solutions (main) $ git checkout dev
Switched to branch 'dev'
Gym-Git-Exercise-Solutions (dev) $ git branch test
Gym-Git-Exercise-Solutions (dev) $ git branch -d test
Deleted branch test (was 5f3c3ff).
Gym-Git-Exercise-Solutions (dev) $ code .
Gym-Git-Exercise-Solutions (dev) $ ^C
Gym-Git-Exercise-Solutions (dev) $ git add .
Gym-Git-Exercise-Solutions (dev) $ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

Gym-Git-Exercise-Solutions (dev) $ git commit -m "Exercise 1 is done"
[dev bde360b] Exercise 1 is done
 1 file changed, 31 insertions(+), 62 deletions(-)
Gym-Git-Exercise-Solutions (dev) $ git checkout main
Switched to branch 'main'
Gym-Git-Exercise-Solutions (main) $ git merge dev
Updating 5f3c3ff..bde360b
Fast-forward
 README.md | 93 +++++++++++++++++++++------------------------------------------
 1 file changed, 31 insertions(+), 62 deletions(-)
Gym-Git-Exercise-Solutions (main) $ git reset
Gym-Git-Exercise-Solutions (main) $ git branch -d dev
Deleted branch dev (was bde360b).
Gym-Git-Exercise-Solutions (main) $ git status
On branch main
nothing to commit, working tree clean
Gym-Git-Exercise-Solutions (main) $ git branch dev
Gym-Git-Exercise-Solutions (main) $ git add .
Gym-Git-Exercise-Solutions (main) $ git commit -m "The exercises containing to create branches and switch through them"
On branch main
nothing to commit, working tree clean
Gym-Git-Exercise-Solutions (main) $ git status
On branch main
nothing to commit, working tree clean


```
### Exercises 2

```bash 

Gym-Git-Exercise-Solutions (main) $ touch home.html
Gym-Git-Exercise-Solutions (main) $ git stash
Saved working directory and index state WIP on main: fa8580e Reset and update README content
Gym-Git-Exercise-Solutions (main) $ touch about.html
Gym-Git-Exercise-Solutions (main) $ git stash pop
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (2fce8625302da174cae010bfe19a87a50b63e0d2)
Gym-Git-Exercise-Solutions (main) $ git stash
Saved working directory and index state WIP on main: fa8580e Reset and update README content
Gym-Git-Exercise-Solutions (main) $ git stash
No local changes to save
Gym-Git-Exercise-Solutions (main) $ git stash about
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'about'
Gym-Git-Exercise-Solutions (main) $ git stash
No local changes to save
Gym-Git-Exercise-Solutions (main) $ touch team.html
Gym-Git-Exercise-Solutions (main) $ git stash
No local changes to save
Gym-Git-Exercise-Solutions (main) $ git reset
Gym-Git-Exercise-Solutions (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Gym-Git-Exercise-Solutions (main) $ ^C
Gym-Git-Exercise-Solutions (main) $ git stash pop
error: Your local changes to the following files would be overwritten by merge:
        README.md
Please commit your changes or stash them before you merge.
Aborting
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.
Gym-Git-Exercise-Solutions (main) $ ^C
Gym-Git-Exercise-Solutions (main) $ git stash -u
Saved working directory and index state WIP on main: fa8580e Reset and update README content
Gym-Git-Exercise-Solutions (main) $ git stash list
stash@{0}: WIP on main: fa8580e Reset and update README content
stash@{1}: WIP on main: fa8580e Reset and update README content
Gym-Git-Exercise-Solutions (main) $ git stash pop stash@{1}
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (b269778c5075a8be0af0afd3f36ea2bd9be59477)
Gym-Git-Exercise-Solutions (main) $

```