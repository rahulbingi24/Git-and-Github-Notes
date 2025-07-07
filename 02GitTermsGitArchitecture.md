## Git Architecture

### 1. **Working Directory**
- The place where you add, edit, and delete files.
  
### 2. **Staging Area (Index)**
- Temporary area where changes are grouped before committing.
  
### 3. **Git Repository (.git folder)**
- Stores all versions (commits), branches, logs, tags, etc.
```
              +--------------------+
              |  Working Directory |
              +--------------------+
                      |
                git add
                      ↓
              +-------------------+
              |   Staging Area    |
              +-------------------+
                      |
              git commit
                      ↓
              +-------------------+
              | Local Repository  |
              +-------------------+
                     |
              git push/pull
                     ↓
              +------+-------------+
              |  Remote Repository |
              +--------------------+
```

If using a remote (e.g., GitHub):

```
              Local Repository
                     |
             git push / pull
                     ↓
              Remote Repository
```

---

## 📖 Git Terminologies

| Term | Description |
|------|-------------|
| **Repository (Repo)** | A directory that contains your project files and `.git` folder |
| **Commit** | A snapshot of your code |
| **Branch** | A parallel version of the repository |
| **Merge** | Combining changes from one branch into another |
| **Clone** | Copying a remote repository to your local machine |
| **Push** | Sending your local commits to the remote repo |
| **Pull** | Getting changes from the remote repo |
| **Stash** | Temporarily shelves changes you’re not ready to commit |
| **HEAD** | A pointer to the latest commit on the current branch |
| **Remote** | A version of your project hosted on a server like GitHub |
| **Fork** | Personal copy of someone else's repository on GitHub |

---


## 🔁 Git Workflow Steps

### 1. **Initialize a Git Repository**
```bash
git init
```

### 2. **Check File Status**
```bash
git status
```

### 3. **Add Files to Staging Area**
```bash
git add <file>
git add .      # Add all changes
```

### 4. **Commit Changes to Repository**
```bash
git commit -m "Your message here"
```

### 5. **View History of Commits**
```bash
git log
```

### 6. **Connect to Remote Repository (e.g., GitHub)**
```bash
git remote add origin <url>
```

### 7. **Push Local Commits to Remote**
```bash
git push origin main
```

### 8. **Pull Latest Changes from Remote**
```bash
git pull origin main
```

---

## 🌿 Branching and Merging Workflow

1. Create a new branch
```bash
git checkout -b feature-branch
```

2. Work on the branch, commit changes.

3. Merge branch into main
```bash
git checkout main
git merge feature-branch
```

4. Delete branch (optional)
```bash
git branch -d feature-branch
```

---

