
# 🧠 Git Commands Cheat Sheet

## ✅ 1. Git Setup
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## ✅ 2. Create or Clone a Repository
```bash
git init                 # Create a new Git repository
git clone <repo-url>     # Clone an existing repo from GitHub or other source
```

## ✅ 3. Basic Git Workflow
```bash
git status               # Check status of files
git add <file>           # Stage a specific file
git add .                # Stage all changes
git commit -m "message"  # Commit staged changes with a message
git log                  # View commit history
```

## ✅ 4. Branching
```bash
git branch               # List branches
git branch <name>        # Create a new branch
git checkout <name>      # Switch to another branch
git checkout -b <name>   # Create and switch to new branch
git merge <branch>       # Merge branch into current one
git branch -d <name>     # Delete a branch
```

## ✅ 5. Remote Repositories
```bash
git remote -v                       # View remote URLs
git remote add origin <url>        # Add a remote repo
git push origin <branch>           # Push branch to remote
git pull origin <branch>           # Pull changes from remote
```

## ✅ 6. Undoing Changes
```bash
git restore <file>                 # Discard local changes
git restore --staged <file>        # Unstage a file
git reset --hard <commit>          # Reset to specific commit
git revert <commit>                # Undo a commit safely
```

## ✅ 7. Tags
```bash
git tag                            # List tags
git tag v1.0                       # Create a tag
git push origin v1.0               # Push a tag to remote
```

## ✅ 8. Stashing Changes
```bash
git stash                          # Save changes temporarily
git stash apply                    # Reapply the stash
git stash list                     # List stashed changes
```

## ✅ 9. Other Useful Commands
```bash
git diff                           # Show file differences
git show <commit>                  # Show changes in a commit
git blame <file>                   # Who changed each line
git fetch                          # Get updates from remote
git rebase <branch>                # Reapply commits on another base
```

## ✅ Daily Workflow Example
```bash
git status
git add .
git commit -m "message"
git pull origin main
git push origin main
```
