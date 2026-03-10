# Industry Level Git Commands

## 1. Git Configuration Commands

### 1. git config --global user.name
**Syntax**
git config --global user.name
**Purpose**
Sets the global username for Git commits.
**Example**
git config --global user.name "VIKRAM-N220575"

### 2. git config --global user.email
**Syntax**
git config --global user.email
**Purpose**
Sets the email associated with commits.
**Example**
git config --global user.email

### 3. git config --list
**Syntax**
git config --list
**Purpose**
Displays all Git configuration settings
**Example**
git config --list

### 4. git config --unset
**Syntax**
git config --unset <key>
**Purpose**
Removes a configuration value from Git settings.
It is used when you want to delete a previously set configuration like username, email, or other settings.
**Example**
git config --global --unset user.name

**ScreenShot**
![alt text](configuration_commands.png)

## 2. Repository setup commands
### 1. git init
**Syntax**
git init
**Purpose**
Initializes a new Git repository in the current directory.
It creates a hidden .git folder that tracks all repository changes.
**Example**
git init

### 2. git clone
**Syntax**
git clone repo-url
**Purpose**
Creates a local copy of an existing remote repository from platforms like GitHub.
It downloads:
the project files
commit history
branches
**Example**
git clone https://github.com/VIKRAM-N220575/GIT_COMMANDS.git

### 3. git clone --branch
**Syntax**
git clone --branch branchname repo-url
**Purpose**
Clones a repository and checks out a specific branch instead of the default branch.
**Example**
git clone --branch main https://github.com/VIKRAM-N220575/GIT_COMMANDS.git

### 4. git clone --depth
**Syntax**
git clone --depth <number> <repository-url>
**Purpose**
Performs a shallow clone, meaning Git downloads only the latest commits instead of the entire history.
This makes cloning much faster.
**Example**
git clone --depth 1 https://github.com/git/git.git

**Screenshot**
![alt text](repository_setup_commands.png)

## Repository status and inspection
### 1. git status
**Syntax**
**Purpose**
**Example**
**Syntax**
git status
**Purpose**
Shows the current state of the repository, including:
modified files
staged files
untracked files
current branch
**Example**
git status

### 2. git log
**Syntax**
git log
**Purpose**
Displays the complete commit history of the repository.
It shows:
commit ID
author
date
commit message
**Example**
git log

### 3. git log --oneline
**Syntax**
git log --oneline
**Purpose**
Shows commit history in short one-line format
**Example**
git log --oneline

### 4. git log --graph
**Syntax**
git log --graph
**Purpose**
Displays commit history as a branch graph visualization.
**Example**
git log --graph --oneline


### 5.  git show
**Syntax**
git show <commit-id>
**Purpose**
Shows detailed information about a specific commit, including changes made.
**Example**
git show HEAD

### 6. git diff
**Syntax**
git diff
**Purpose**
Shows differences between working directory and staging area.
**Example**
git diff

### 7. git diff --staged
**Syntax**
git diff --staged
**Purpose**
Shows differences between staged files and last commit.
**Example**
git diff --staged

### 8. git blame
**Syntax**
git blame <file>
**Purpose**
Shows who last modified each line of a file.
**Example**
git blame index.hmtl

### 9. git reflog
**Syntax**
git reflog
**Purpose**
Shows a history of all HEAD movements (branch switches, resets, commits).
Very useful for recovering lost commits
**Example**
git reflog

### 10. git shortlog
**Syntax**
git shortlog
**Purpose**
Displays a summary of commits grouped by author.
**Example**
git shortlog

**Screenshots**
![alt text](repo_status&inspection-1.png) 
![alt text](repo_status&inspection-2.png)
![alt text](repo_status&inspection-3.png)

## File Tracking Commands
### 1. git add
**Syntax**
git add <file-name>
**Purpose**
Adds a specific file to the staging area so it can be included in the next commit.
**Example**
git add repo_status&inspection-1.png

### 2. git add .
**Syntax**
git add .
**Purpose**
Adds all modified and new files in the current directory to the staging area.
**Example**
git add .

### 3. git add -p
**Syntax**
git add -p
**Purpose**
Allows you to stage changes interactively.
You can choose which parts (hunks) of the file should be added to staging.
**Example**
git add -p

### 4. git restore
**Syntax**
git restore <file-name>
**Purpose**
Discards changes in the working directory and restores the file to the last committed version.
**Example**
git restore index.html

### 5. git restore --staged
**Syntax**
git restore --staged <file-name>
**Purpose**
Removes a file from the staging area but keeps the changes in the working directory.
**Example**
git restore --staged index.html

### 6. git rm
**Syntax**
git rm <file-name>
**Purpose**
Deletes a file from the working directory and Git repository.
**Example**
git rm test.txt

### 7. git mv
**Syntax**
git mv <old-name> <new-name>
**Purpose**
Moves or renames a file and stages the change automatically.
**Example**
git mv oldfile.txt newfile.txt

**Screenshots**