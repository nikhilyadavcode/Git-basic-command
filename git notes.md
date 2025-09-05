# 📘 Git Notes (Complete Cheat Sheet)

Git is a **distributed version control system** used to track changes in source code and collaborate with others.

---

## 🔹 1. Git Basics

- `git init` → Initialize a new Git repository in the current directory (creates `.git` folder).
- `git clone <repo_url>` → Clone (copy) an existing repository to your machine.
- `git status` → Show status of files (modified, staged, untracked).
- `git diff` → Show the changes in files that are not yet staged for commit.

---

## 🔹 2. Staging & Committing

- `git add file.txt` → Add a file to the staging area.
- `git add .` → Add **all modified and new files** to staging.
- `git commit -m "Message"` → Commit staged changes with a message.
- `git commit -am "Quick commit"` → Add & commit all tracked files (skip `git add`).

---

## 🔹 3. Branching

- `git branch` → List all branches.
- `git branch feature-x` → Create a new branch.
- `git checkout feature-x` → Switch to a branch.
- `git switch feature-x` → Newer alternative for switching branches.
- `git checkout -b feature-x` → Create & switch to a branch at once.
- `git branch -d feature-x` → Delete a branch safely.

---

## 🔹 4. Merging & Rebasing

- `git merge feature-x` → Merge branch into current branch.
- `git rebase main` → Reapply commits on top of another branch (linear history).
- `git rebase --abort` → Cancel a rebase.

---

## 🔹 5. Remote Repositories

- `git remote add origin <url>` → Add remote repository (e.g., GitHub).
- `git remote -v` → Show linked remotes.
- `git push origin main` → Push commits to remote.
- `git pull origin main` → Pull latest changes from remote.
- `git fetch` → Download changes without merging.

---

## 🔹 6. Undoing Changes

- `git reset file.txt` → Unstage a file.
- `git reset --soft HEAD~1` → Undo last commit, keep changes staged.
- `git reset --hard HEAD~1` → Undo last commit, discard changes.
- `git checkout -- file.txt` → Discard local file changes.
- `git revert <commit_id>` → Undo a commit safely (creates a new commit).

---

## 🔹 7. Viewing History

- `git log` → Show detailed commit history.
- `git log --oneline` → Short one-line history.
- `git log --oneline --graph --all` → Branch graph view.
- `git show <commit_id>` → Show details of a commit.

---

## 🔹 8. Stashing

- `git stash` → Save uncommitted changes temporarily.
- `git stash list` → Show all stashes.
- `git stash apply` → Reapply last stash (keeps it).
- `git stash pop` → Apply last stash and remove it.

---

## 🔹 9. Tags

- `git tag v1.0` → Create a lightweight tag.
- `git tag -a v1.0 -m "Version 1.0 release"` → Create an annotated tag.
- `git push origin --tags` → Push tags to remote.

---

## 🔹 10. Useful Shortcuts & Tips

- `git show HEAD` → Show details of last commit.
- `git diff branch1 branch2` → Compare two branches.
- `git clean -f` → Remove untracked files.
- `git commit --amend` → Edit last commit.


 ## 🔹 Key Commands for Getting Help
- `git help <command>` - See the manual page for a command
-`git <command>` --help - See help for a command (same as above)
-`git <command>` -h - See a quick summary of options
-`git help --all` - List all possible Git commands
-`git help -g` - List guides and concepts

## 🔹 Git Branch
- Rename a branch: `git branch -m old-name new-name`
- List all branches:` git branch`
- Switch branches: `git checkout branch-name or git switch branch-name`
- Delete a branch (not merged): `git branch -D branch-name`
- See which branch you're on:` git status`

## 🔹 Common git merge Options
- `git merge` - Merge a branch into your current branch
- `git merge `--no-ff - Always create a merge commit
- `git merge` --squash - Combine changes into a single commit
- `git merge` --abort - Abort a merge in progress

## 🔹 Git Workflow Commands Overview
- `Working Directory` - Where you make changes
- `git add` - Stage changes
- `git commit` - Save changes to your repository
- `git push `- Share changes with others
- `git status` - Check what's going on
- `Undo/Amend` - Fix mistakes (git restore, git reset, git commit --amend)

## 🔹 Summary of Git Terms
Branch
Checkout
Clone
Commit
Conflict
Fetch
Fork
HEAD
Index (Staging Area)
Merge
Origin
Pull
Push
Rebase
Remote
Repository (Repo)
Stash
Tag
Upstream
Working Directory