# Git Cheat Sheet - Branch NewLook

### Configuration

- `git config --global user.name "[name]"` and `git config --global user.email "[email address]"`: Set your name and email for commit transactions.
- `git config --global color.ui auto`: Enables color in the command line output for better readability.

### Creating Repositories

- `git init [project-name]`: Initializes a new local Git repository.
- `git clone [url]`: Copies a project and its full history from a remote URL.

### Making Changes

- `git status`: Shows which files are new or modified and need to be committed.
- `git diff`: Displays changes in files that are not yet staged.
- `git add [file]` or `git add .`: Stages specific files or all changes for the next commit.
- `git commit -m "[descriptive message]"`: Saves the staged changes to the repository's history with a message.
- `git commit --amend`: Modifies the most recent commit. 

### Grouping Changes (Branching)

- `git branch`: Lists your local branches.
- `git branch [branch-name]`: Creates a new branch.
- `git checkout [branch-name]` or `git checkout -b <new-branch-name>`: Switches to an existing branch or creates and switches to a new one.
- `git merge [branch]`: Integrates changes from a specified branch into your current branch.
- `git branch -d [branch]`: Deletes a specific branch.

### Review History

- `git log` or `git log --oneline`: Shows the commit history in detail or a condensed format.
- `git show [commit]`: Displays information and changes for a specific commit.

### Synchronizing Changes

- `git fetch [bookmark]`: Downloads history from a remote but doesn't integrate changes.
- `git pull`: Downloads and integrates changes from a remote (fetch and merge).
- `git push`: Uploads your local branch's commits to a remote repository.
- `git remote add [remote] [url]`: Adds an alias for a remote repository.

### Suppressing Tracking

- **`.gitignore`**: Use this file to prevent Git from tracking specified files or directories.

### Temporary Commits

- `git stash`: Temporarily saves changes to tracked files.
- `git stash pop`: Restores the most recently stashed changes and removes the stash entry.