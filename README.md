# Elzero Git Course Summery

### 03 : Create GitHub Repository And Clone It
    git clone "Your Repository URL"

### 04 - Add, Reset, Commit And Progress
    # Add Files
    git add <File> <File>
    git add *.extension
    git add *

    # Show Status
    git status

    # Commit Changes
    git commit -m "Commit Message Here"

### 05 - Push Local Changes To Remote Repository
    # Show Branches
    git branch
    git remote -v

    # Push Changes
    git push origin main

    # Add Files
    git add <File> <File>

    # Commit Changes
    git commit -m "Commit Message Here"

### 06 - Pull Changes From Remote Repository
    # Pull Changes From Remote Repository
    git pull origin

### 07 - Everything About Git Configurations
    # Show All Configurations
    git help config

    # Show User Email
    git config --global user.email

    # Change User Email
    git config --global user.email "Your Github Email Here"

    # Edit Configuration
    git config --global --edit

    # Create New File
    touch "File Name Here"

### 08 - Generate And Test Github Public Key
    # Generate Key
    ssh-keygen -t rsa -b 4096 -C "Your GitHub Email Here"

    # Get Key To Copy
    cat ~/.ssh/id_rsa.pub

    # Same Command Example in Windows "Change Osama With Your Username"
    cat C:\Users\osama\.ssh\id_rsa.pub

    # Test Key And Connection
    ssh -T git@github.com

### 09 - Create Repository From Existing Project
    # Create New Directory
    mkdir "Your Directory Name Here"

    # Initialize Empty Git Repository
    git init

    # Create Empty File
    touch "Your File Name Here"

    # Show Status
    git status

    # Add Files
    git add <File> <File>

    # Commit File
    git commit -m "Your Commit Message Here"

    # Add Repository
    git remote add origin "SSH Repository URL"

    # Example
    git remote add origin "git@github.com:OsamaElzero/Course.git"

    # Push Data
    git push -u origin master

### 11 - Everything About Aliases
    # Make Alias For Command "status"
    git config --global alias.st status

    # Show Alias Content
    git config --global alias.st

    # Test "status" Command
    git st

    # Make Alias For Command "branch"
    git config --global alias.br branch

    # Show Alias Content
    git config --global alias.br

    # Test "branch" Command
    git br

    # Make Alias For Command "commit -m"
    git config --global alias.cm "commit -m"

    # Show Alias Content
    git config --global alias.cm

    # Test "branch" Command
    git cm

    # Show All Edits
    git config --global --edit

### 12 - Branching And Merging
    # Show Branches
    git branch

    # Switch To Branch
    git checkout "Branch Name"

    # Delete Branch
    git branch -d "Branch Name"

    # Create Branch And Switch To It
    git checkout -b "Branch Name"

    # Move / Rename Branch
    git branch -m "New Branch Name"

    # Merge Branch With Current Branch
    git merge "Branch Name You Need To Merge"

### 13 - Mastering Stash Part 1
    # Create Text File With "Hello World" String Inside It
    echo "Hello World" > about_readme.txt

    # Save Work To Stash
    git stash

    # List Items in Stash
    git stash list

    # Get Work From Stash
    git stash pop

### 14 - Mastering Stash Part 2
    # Save Work To Stash
    git stash

    # List Items in Stash
    git stash list

    # Get Work From Stash
    git stash pop

    # Save Work To Stash With Description
    git stash save "Description Here"

    # Get Specific Stash
    git stash pop stash@{2}

    # Delete Stash
    git stash drop stash@{1}

    # Show Lastest Added Stash Content
    git stash show

    # Show Specific Stash Content
    git stash show stash@{1}

    # Empty The Stash
    git stash clear

### 15 - Restore And Clean
    # Restore Staged Files
    git restore --staged "File Name Here"

    # Show Files That Will Be Cleaned
    git clean -n

    # Remove Un Needed Files
    git clean -f

### 16 - Resetting The Head
    # Show Log File
    git log

    # Reset Head
    git reset --hard "Commit Hash Here"

    # Push Edits From Local To Remote With Force Flag
    git push origin main --force

### 17 - Ignoring Files And Directories
    *.log
    !vip.log
    node_packs/
    text.txt

### 18 - Tagging And Releasing Part 1
    # Show All Tags
    git tag

    # Add New Lightweight Tag
    git tag "Version Name Or Tag Name Here"

    # Add New Annotated Tag
    git tag -a "Version Name Or Tag Name Here" -m "Description Or Message"

    # Push Tag To Remote
    git push origin "Tag Name Here"

### 19 - Tagging And Releasing Part 2
    # List All Tags Starting With v1.
    git tag -l "v1.*"

    # Delete Tag
    git tag -d "Version Name Or Tag Name Here"

    # Delete Tag From Remote
    git push origin --delete "Version Name Or Tag Name Here"

### 20 - The End And Advices
Git [Handbook](https://www.amazon.com/Git-Version-Control-Cookbook-Productivity/dp/1782168451) 
