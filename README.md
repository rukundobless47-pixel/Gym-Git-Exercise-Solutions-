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

## bundel 2

### Exercises 1

```bash
Gym-Git-Exercise-Solutions (main) $ git branch ft/bundel-2
Gym-Git-Exercise-Solutions (main) $ git checkout ft/bundel-2
M       README.md
Switched to branch 'ft/bundel-2'
Gym-Git-Exercise-Solutions (ft/bundel-2) $ touch services.html
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git add services.html
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git commit -m "I have added the new file"
[ft/bundel-2 b9eda8d] I have added the new file
 1 file changed, 13 insertions(+)
 create mode 100644 services.html
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git checkout main
M       README.md
Switched to branch 'main'
Gym-Git-Exercise-Solutions (main) $ giti push ^C
Gym-Git-Exercise-Solutions (main) $ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Gym-Git-Exercise-Solutions (main) $ git checkout ft/bundel-2
M       README.md
Switched to branch 'ft/bundel-2'
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git push -u origin ft/bundel-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 520 bytes | 260.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/bundel-2' on GitHub by visiting:
remote:      https://github.com/rukundobless47-pixel/Gym-Git-Exercise-Solutions-/pull/new/ft/bundel-2
remote:
To https://github.com/rukundobless47-pixel/Gym-Git-Exercise-Solutions-.git
 * [new branch]      ft/bundel-2 -> ft/bundel-2
branch 'ft/bundel-2' set up to track 'origin/ft/bundel-2'.
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git status
On branch ft/bundel-2
Your branch is up to date with 'origin/ft/bundel-2'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Gym-Git-Exercise-Solutions (ft/bundel-2) $ git diff README.md
diff --git a/README.md b/README.md
index 794ed27..3017b13 100644
--- a/README.md
+++ b/README.md
@@ -152,4 +152,13 @@ no changes added to commit (use "git add" and/or "git commit -a")
 Dropped stash@{1} (b269778c5075a8be0af0afd3f36ea2bd9be59477)
 Gym-Git-Exercise-Solutions (main) $

```
## bundel 2

### Exercises 1

```bash
This is about exercises 1 in this bundel
 
```
