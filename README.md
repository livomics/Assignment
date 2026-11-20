
Olivia Balys 20-11-2026
Student of Bioinformatics 3rd year testing git out:p

---

## Setup & SSH
Huge appreciation for having clear instructions on how to set up SSH and Git together—managed to get it working on the very first try.

- ls -al ~/.ssh - lists your ssh keys
- ssh-keygen -t ed25519 -C "your-email@example.com - to create a new key 
- cat ~/.ssh/id_ed25519.pub - to show your new made key 
- `git config --global user.name "Your Name"` — Sets the author name attached to your commits.
- `git config --global user.email "you@example.com"` — Sets the email address attached to your commits.
- `ssh -T git@github.com` — Tests the SSH connection to verify authentication works without a password.

---

## Basic Commands
* `git clone <linkfromgitssh>` - clones the repo from github
* `git status` — Shows modified files, staged changes, and the current branch.
* `git add <file>` (or `git add .`) — Puts changes in a box so they are ready for the next commit.
* `git commit -m "message"` — Saves staged changes to the local repository history with a descriptive note.
* `git push` — Uploads local commits to the remote repository (e.g., GitHub).
* `git pull` — Downloads changes from the remote repository and merges them into your current branch.
* `git log` — Displays the commit history (add `--oneline` for a compact view).

##Basic but more geeky
* `git branch` — Lists all local branches (or creates a new one with `git branch <name>`).
* `git diff` — Shows line-by-line differences between unstaged changes and the last commit.
* `git merge <branch>` — Combines the history and changes of `<branch>` into your currently active branch.


## Commands That Do Almost the Same Thing

### Switching Branches
* `git switch <branch>` — The modern, dedicated command solely for moving between branches (use `-c` to create and switch).
* `git checkout <branch>` — The older, multi-purpose command used to switch branches, though it can also restore files.

### Getting Remote Updates
* `git fetch` — Downloads new data from the remote repository so you can inspect it, without altering your local working files.
* `git pull` — Runs `git fetch` followed immediately by `git merge` to update your local branch right away (this is what AI said). I would say that git pull is like git fetch but changes what you have localy.
    

## Restoring Changes

* `git restore <file>` — Discards unstaged changes in your working directory, reverting the file back to the last commit.

When you go back to see how your worked looked like, you cannot modify it. You have to branch it first and then you can work on it.

