# Git-Github

📝 Basic Git Workflow & Key Concepts
✅ >>> git init

What it does:
Initializes an empty Git repository in your current folder. It creates a hidden .git/ directory.

✅ 2. Untracked vs Unstaged Files
When you create a new file (e.g., hello.txt), it's:
Untracked – Git doesn’t know it yet.

>>> git status (it helps to check status in the sense file is tracked or staged or modified or committed)
----> initially the file is untracked once you run the git add . command the git started to track (staged) the file


✅ 3. git add .
Command:
git add .
What it does:

Adds all untracked and modified files to the staging area.

Files are now staged and ready to commit.


if we modify nything in the file the git tracks and when we check status it shows modified
-->in this case it is unstaged so we have to again run >>>git add .    (or) >>>git add filename

✅ 4. git commit
Command:

git commit -m "Initial commit"
What it does:

Takes a snapshot of all staged files.

Adds it to Git’s history as a commit.

🔄 Git File Lifecycle Summary
| State     | Description                | Command to Move to Next State |
| --------- | -------------------------- | ----------------------------- |
| Untracked | New file, not known to Git | `git add filename`            |
| Unstaged  | Known to Git but modified  | `git add filename`            |
| Staged    | Ready to commit            | `git commit`                  |
| Committed | Saved in Git history       | –                             |

✅ 5.branching stratergy

>>> git branch -m main
---> to create main branch
---> this main branch includes production ready code (so don't directly push to main branch)

>>> git checkout -b vinay(branch_name)
---->this is to create feature branch and to enter in that

>>> git branch branch_name
---->if we just want create branch name

push to whichever branch you want 
>>> git push -u origin branchname

✅ 6. clone vs pull

# Clone once (it copy the repo from remote to local)
# use this when you are first time working
>>> git clone https://github.com/user/repo.git

# Later, pull updates from remote
#if we make any changes in global repo it doesn't appear in local ,so pull updates in local repo
>>> git pull origin main






