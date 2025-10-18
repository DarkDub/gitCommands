# Git Commands

##  Basic Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
git config --list
````

---

##  Starting a Repository

```bash
git init                      # Initialize a new repository
git clone <url>               # Clone an existing repository
```

---

##  Staging and Committing

```bash
git status                    # Show current changes
git add <file>                # Add a specific file
git add .                     # Add all files
git commit -m "message"       # Commit with message
git commit -am "message"      # Add + commit in one command
```

---

##  Branch Management

```bash
git branch                    # List all branches
git branch <name>             # Create a new branch
git checkout <branch>         # Switch to a branch
git checkout -b <branch>      # Create and switch to a branch
git merge <branch>            # Merge another branch
git branch -d <branch>        # Delete a branch
```

---

##  Remote Repositories

```bash
git remote -v                 # Show connected remotes
git remote add origin <url>   # Connect to remote
git push -u origin main       # Push first commit
git push                      # Push changes
git pull                      # Pull latest changes
git fetch                     # Fetch updates (no merge)
```

---

##  Undoing Changes

```bash
git restore <file>            # Undo unstaged changes
git restore --staged <file>   # Unstage a file
git reset --hard HEAD         # Reset to last commit
git reset --hard <commit>     # Reset to specific commit
git revert <commit>           # Undo commit safely (creates new commit)
```

---

##  Commit History

```bash
git log                       # Show commit history
git log --oneline             # Compact view
git diff                      # Show unstaged changes
git diff --staged             # Show staged changes
```

---

##  Tagging Versions

```bash
git tag                       # List all tags
git tag <tagname>             # Create a tag
git tag -a <tagname> -m "msg" # Annotated tag
git push origin <tagname>     # Push a specific tag
git push origin --tags        # Push all tags
```

---

##  Working with GitHub

```bash
git remote add origin <url>   # Link local repo to GitHub
git push -u origin main       # Push main branch
git push origin <branch>      # Push a specific branch
git pull origin main          # Pull latest version from GitHub
```

---

##  Stash (Save Temporary Changes)

```bash
git stash                     # Save uncommitted changes
git stash list                # Show stashes
git stash apply               # Apply last stash
git stash pop                 # Apply + remove last stash
```

---

##  Useful Shortcuts

```bash
git shortlog -sn              # Show commits per author
git show <commit>             # Show specific commit details
git blame <file>              # Show who changed each line
```

---

##  Advanced Commands

```bash
git cherry-pick <commit>      # Apply specific commit from another branch
git rebase <branch>           # Move commits to another base branch
git reflog                    # Show all actions (even deleted commits)
git clean -f                  # Remove untracked files
```

---

##  Authentication Tips

```bash
git config --global credential.helper store   # Save credentials permanently
git config --global credential.helper cache   # Cache temporarily
```

---

##  Common Workflows

### Push Local Repo to GitHub (first time)

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main
```

### Update Repo with Latest Changes

```bash
git pull origin main
git add .
git commit -m "Update project"
git push
```



