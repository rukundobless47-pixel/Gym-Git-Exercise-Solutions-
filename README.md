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