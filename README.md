# 🧠 Git Cheatsheet

## 1. What is Git?
- Git is a **version control system**.
- It tracks code changes and helps collaborate.
- Allows you to revert to previous versions of your code.

## 2. Git vs GitHub
- **Git**: Local tool to track changes.
- **GitHub**: Online platform to host and share Git repositories.

## 3. Installation & Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## 4. Basic Git Commands
| Command | Description |
|---------|-------------|
| `git init` | Initialize a Git repository |
| `git status` | Show changes in your repo |
| `git add file.txt` | Stage a file |
| `git commit -m "message"` | Save a snapshot |
| `git log` | Show commit history |
| `git diff` | View file differences |
| `git clone <url>` | Copy a remote repo locally |
| `git pull` | Fetch and merge changes from remote |
| `git push` | Upload local changes to remote |

## 5. The Git Workflow
```text
Working Directory → Staging Area → Repository
```
```bash
git add .
git commit -m "your message"
git push origin main
```

## 6. Branching & Merging
```bash
git branch new-feature
git checkout new-feature
git merge main
```
- Branches allow you to test features safely.
- Merge changes back into the main branch.

## 7. .gitignore
Use `.gitignore` to exclude files from being tracked.
```plaintext
*.log
__pycache__/
.env
```

## 8. Undoing Changes
```bash
git checkout -- file.txt      # Discard local changes
git reset HEAD file.txt       # Unstage a file
git revert <commit_hash>      # Revert a commit
```

## 9. Working with GitHub
- Create a GitHub repo.
- Clone the repo:
```bash
git clone https://github.com/user/repo.git
```
- Make changes → commit → push:
```bash
git push origin main
```
- Open Pull Requests, use Issues to track tasks.

## 🛠️ Practice Ideas
- Create a repo and make commits.
- Create and merge branches.
- Collaborate with a teammate using GitHub.

## 🧩 Bonus Concepts
- `git stash`: Save changes temporarily.
- `git rebase`: Rewrite commit history.
- Git GUIs: VS Code Git Panel.

