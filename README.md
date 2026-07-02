# git Exercises

## Bundel 1

### Exercises 1

```bash
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git init 
Reinitialized existing Git repository in C:/Users/rukun/OneDrive/Desktop/The Gym/TheGym_git_exercises/Gym-Git-Exercise-Solutions/.git/
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git branch -M master
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> 
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> 
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git commit -m"chaed from main to master"
[master (root-commit) 6b3333d] chaed from main to master
 1 file changed, 7 insertions(+)
 create mode 100644 README.md
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> 
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git status
On branch master
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git init
Reinitialized existing Git repository in C:/Users/rukun/OneDrive/Desktop/The Gym/TheGym_git_exercises/Gym-Git-Exercise-Solutions/.git/
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git commit -m"exercises 1" 
[master 712fef8] exercises 1
 1 file changed, 1 deletion(-)
PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:main

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.

PS C:\Users\rukun\OneDrive\Desktop\The Gym\TheGym_git_exercises\Gym-Git-Exercise-Solutions> 
```
