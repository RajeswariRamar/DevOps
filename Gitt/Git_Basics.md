# Git & GitHub – Quick Setup Guide

## 1. Create a New GitHub Repository

1. Open https://github.com
2. Click **+ → New repository**
3. Repository name: `DevOps-Practice`
4. Select Public or Private.
5. Tick **Add a README file**.
6. Click **Create repository**.

## 2. Clone the Repository to a New Windows Path

Open Git Bash and run:

```bash
cd /c/Users/HP
git clone https://github.com/RajeswariRamar/DevOps-Practice.git
cd DevOps-Practice
```

**Local path:**
`C:\Users\HP\DevOps-Practice`

All my project files and folders should be created inside this directory.

## 3. Configure Git (Only Once Per Computer)

```bash
git config --global user.name "RajeswariRamar"
git config --global user.email "YOUR_EMAIL"
```

## 4. Create and Push a New Branch

```bash
git checkout -b master
git push -u origin master
```

If `master` already exists, use:

```bash
git checkout master
```

## 5. Create DevOps Practice Folders

```bash
mkdir Linux Git Docker Jenkins
```

## 6. Check Repository Status

```bash
git status
git branch
git remote -v
```

## 7. Upload Changes to GitHub

Whenever I create or modify files, run:

```bash
git add .
git commit -m "Add DevOps practice files"
git push
```

- `git add .` – Stage new and modified files.
- `git commit -m "message"` – Save the staged changes locally.
- `git push` – Upload committed changes to GitHub.

**Important:** Run these commands from inside the repository folder. If there are no changes, Git may say there is nothing to commit.

## 8. Daily Workflow

```bash
cd /c/Users/HP/DevOps-Practice
git status
git pull
# Create or modify files
git add .
git commit -m "Describe my changes"
git push
```

## Remember

- GitHub = Remote repository.
- Local folder = Files on my computer.
- Git Bash = Terminal to run Git commands.
- Branch = Separate line of development.
- `add → commit → push` = Stage → Save locally → Upload to GitHub.
- Saving a file on Windows does NOT automatically upload it to GitHub.
- Use `git pull` before starting work to get the latest remote changes.
