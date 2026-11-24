# Session 1 Reflection
**Name:** Norman Yusoff
**Student ID:** 97640

## Q1. Why is a commit history useful when maintaining software?
A commit history acts as a detailed timeline of every change made to a project, recording what was modified, when it happened, and who made the change. In a real maintenance situation, such as discovering a bug after a recent update, developers can inspect the log to pinpoint the exact commit that introduced the error and roll it back safely. For example, in my `scm-lab-evidence-97640` repository, commits like `Add .gitignore` and `Add Session 1 notes` clearly separate each task. If a configuration issue appeared later, I could trace it directly to the specific commit instead of guessing which file broke.

## Q2. Difference between Git and GitHub
Git is the local version control software installed on my computer that tracks file changes, manages branches, and stores commit history offline. GitHub is an online hosting platform that stores remote copies of Git repositories and adds collaboration tools like pull requests and automated checks. In this lab, I used Git locally to initialize my repository, stage files, and merge branches on my machine. I then used GitHub both to complete the browser-based GitHub Skills exercise repository and to host `scm-lab-evidence-97640` online so a simulated teammate could clone and push changes.

## Q3. What risk does using a branch and pull request reduce?
Working on a separate branch and merging through a pull request reduces the risk of breaking the stable `main` branch with untested or incomplete code. It isolates new changes so they can be reviewed, tested, and verified by teammates or automated checks before becoming part of the main codebase. In the GitHub Skills exercise, this workflow ensured that my new file was checked before merging rather than overwriting `main` directly.

## Q4. Local commands vs. GitHub commands
Commands that changed only my local computer included `git init`, `git add`, `git commit`, `git switch`, `git merge`, `git branch -d`, and `git restore`, because they only modified my working directory, staging area, and local repository history. Commands that interacted with and changed GitHub were `git push` (which uploaded my local commits to the remote repository), while `git clone` and `git pull` downloaded data from GitHub to my computer without altering the remote repository itself.

## Concept Table (Part 1)

| Term | Definition |
|---|---|
| Repository | A project folder along with its complete commit history and version tracking data. |
| Working tree (working directory) | The actual files and folders currently checked out on your computer that you view and edit. |
| Staging area (index) | A holding area listing the specific changes selected to be included in the next commit. |
| Commit | A saved snapshot of staged changes in the repository, recorded with a message, author, and date. |
| Branch | A movable pointer to a specific line of commits, allowing parallel development without affecting `main`. |
| Merge | The process of combining the commit history and changes from one branch into another. |
| Remote | A hosted copy of a repository stored on another server, such as `origin` on GitHub. |
| Push / Pull / Clone | Push uploads local commits to a remote; pull downloads and merges remote commits; clone copies a remote repository to your computer for the first time. |
