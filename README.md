# Git Commands Cheatsheet

## Table of Contents
1. [Getting Help](#getting-help)
2. [Configuration](#configuration)
3. [Basic Commands](#basic-commands)
4. [Working with Files](#working-with-files)
5. [Committing Changes](#committing-changes)
6. [Undoing Changes](#undoing-changes)
7. [Working with Remotes](#working-with-remotes)
8. [Branching](#branching)
9. [Merging](#merging)
10. [Tagging](#tagging)
11. [Advanced Commands](#advanced-commands)

## Getting Help
1. `git help`: Take help from GitHub help section for different commands and other errors

## Configuration
2. `git config`: To set the basic configurations on GitHub like your name and email
3. `git config --global user.name "username"`: Sets configuration values for your user name on Git
4. `git config --global user.email name@gmail.com`: Sets configuration values for your user email on Git
5. `git config --global color.ui true`: To see different colors on command line for different outputs

## Basic Commands
6. `mkdir store`: Create a directory if not created initially
7. `cd store`: To go inside the directory and work upon its contents
8. `git init`: To create a local git repository for us in our store folder
9. `git status`: To see what's changed since last commit
10. `ls`: To see directories and files in the current directory

## Working with Files
11. `git add Readme.txt`: To add a file Readme.txt to the staging area to track its changes
12. `git add`: To add a specific list of files to staging area
13. `git add --all`: To add all files of current directory to staging area
14. `git add *.txt`: To add all text files of the current directory to staging area
15. `git add docs/*.txt`: To add all text files of a particular directory(docs) to staging area
16. `git add docs/`: To add all files in a particular directory(docs) to staging area
17. `git add "*.txt"`: To add text files of entire project to staging area

## Committing Changes
18. `git commit -m "Created a Readme.txt"`: To commit our changes and provide a message
19. `git log`: To check the history of commits for our reference
20. `git diff`: To figure out what changes you made since last commit
21. `git commit -a -m "Readme.md"`: To add any of our tracked files to staging area and commit them

## Undoing Changes
22. `git reset head license`: To undo staging of the file that was added in the staging area
23. `git checkout --license`: To blow away all changes since the last commit of the file
24. `git reset --soft HEAD^`: To undo last commit and bring file to staging area
25. `git reset --hard HEAD^`: To undo last commit and remove file from the staging area
26. `git reset --hard HEAD^^`: To undo last 2 commits and all changes

## Working with Remotes
27. `git remote add origin https://....`: To add a remote named 'origin' pointing to the given URL
28. `git remote add <address>`: To add new remotes to our local repository for a particular git address
29. `git remove rm`: To remove a remote from our local repository
30. `git push -u origin master`: To push contents of local master branch to the server
31. `git clone https://....`: To clone a global repository to your local system
32. `git fetch`: To fetch down any changes from global repository to current repository

## Branching
33. `git branch Testing`: To create a new branch named 'Testing'
34. `git branch`: To see all branches and the current branch
35. `git checkout Testing`: To switch to branch 'Testing' from master branch
36. `git checkout -b admin`: To create a new branch 'admin' and set it as current branch
37. `git branch -r`: To look at all the remote branches
38. `git branch -d Testing`: To delete 'Testing' branch
39. `git branch -D Testing`: To forcefully delete a branch without making commits

## Merging
40. `git merge Testing`: To merge 'Testing' branch with master branch

## Tagging
41. `git tag`: To see the list of available tags
42. `git checkout v0.0.1`: To set the current tag to v0.0.1
43. `git tag -a v0.0.3 -m "version 0.0.3"`: To create a new tag
44. `git push --tags`: To push the tags to remote repository

## Advanced Commands
45. `git rebase`: Move all changes to master which are not in origin/master to a temporary area, run all origin master commits, then run all commits in the temporary area on top of our master one at a time

## Additional Resources
Video demonstration: [Git Commands Tutorial](https://drive.google.com/drive/folders/1H-e-BxtHejbAq2eOd_Np8D1Z1-Pepz62?usp=sharing)
