
#**Git Commands Reference**

This document contains a comprehensive list of common Git commands for version control.

**Configuring Git**

- Set up your name and email (Global configuration)
  - git config --global user.name "Your Name"
  - git config --global user.email "you@example.com"

- Check your configuration
  - git config --list

- Set up default text editor
  - git config --global core.editor "vim"

**Creating and Cloning Repositories**

- Initialize a new Git repository
  - git init

- Clone a remote repository
  - git clone <repository_url>

**Working with Changes**

- Check the status of the repository
  - git status

- Stage a file for commit
  - git add <file_name>

- Stage all changes for commit
  - git add .

- Unstage a file
  - git reset <file_name>

- Commit changes
  - git commit -m "Your commit message"

- Commit all changes with a message
  - git commit -a -m "Your commit message"

- View commit history
  - git log

- View commit history (one line per commit)
  - git log --oneline

**Working with Branches**

- Create a new branch
  - git branch <branch_name>

- List all branches
  - git branch

- Switch to a branch
  - git checkout <branch_name>

- Create and switch to a new branch
  - git checkout -b <branch_name>

- Merge another branch into the current branch
  - git merge <branch_name>

- Delete a branch
  - git branch -d <branch_name>

- Delete a remote branch
  - git push origin --delete <branch_name>

**Remote Repositories**

- View remote repositories
  - git remote -v

- Add a remote repository
  - git remote add origin <repository_url>

- Remove a remote repository
  - git remote remove origin

- Push changes to a remote repository
  - git push origin <branch_name>

- Pull changes from a remote repository
  - git pull origin <branch_name>

- Fetch updates from the remote without merging
  - git fetch

- Push tags to a remote repository
  - git push --tags

**Working with Tags**

- List all tags
  - git tag

- Create a tag
  - git tag <tag_name>

- Tag a specific commit
  - git tag <tag_name> <commit_hash>

- Delete a tag
  - git tag -d <tag_name>

- Push a tag to remote
  - git push origin <tag_name>

**Undoing Changes**

- Undo changes in a file (working directory)
  - git checkout -- <file_name>

- Remove a file from the staging area
  - git reset <file_name>

- Undo the last commit but keep the changes staged
  - git reset --soft HEAD~1

- Undo the last commit and unstage the changes
  - git reset --mixed HEAD~1

- Undo the last commit and discard changes
  - git reset --hard HEAD~1

- Revert a commit (creates a new commit)
  - git revert <commit_hash>

- Remove untracked files
  - git clean -f

**Stashing Changes**

- Save changes for later (stash)
  - git stash

- Apply the most recent stash
  - git stash apply

- List all stashes
  - git stash list

- Drop a stash
  - git stash drop

- Apply and drop the most recent stash
  - git stash pop

**Git Diff**

- Show changes between working directory and the index (staged changes)
  - git diff

- Show changes between the index and the last commit
  - git diff --cached

- Show changes between two commits
  - git diff <commit_hash_1> <commit_hash_2>

**Other Useful Commands**

- Show the current branch
  - git rev-parse --abbrev-ref HEAD

- Show the last commit
  - git show

- Show file history
  - git log <file_name>

- Show commit changes in a file
  - git log -p <file_name>

- Show the commit difference between two branches
  - git diff <branch_1>..<branch_2>

**Git Help**

- Get help for any Git command
  - git help <command>

- Get help for a specific sub-command
  - git <command> --help

**Configuration and Troubleshooting**

- Check the current configuration
  - git config --list

- Debug and show Git internal information
  - git fsck

- Show all the branches in the repository (including remote branches)
  - git branch -a

**Git Aliases**

- Set a custom alias for a command
  - git config --global alias.st status
  Now you can use `git st` instead of `git status`.

- List all aliases
  - git config --global --get-regexp alias

---

This list includes the most commonly used Git commands to help you get started and work efficiently with Git repositories.
