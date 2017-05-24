# git for beginners

  * Git is used to track the versions of files. It is a distributed version control system VCS
  * SCM - Source Code Management
  * SVN - Centralized Version control System - Source code & versions are in central server. SVN client checkout code & working on that. Each commits happens on the central repository.
  * GIT - Distributed Version Control System. Each developer has their own repository. Each commit happens in locally. Then finally push their code into remote repository
  
# GIT setup 

 * Install git in your machine
 * git config --global user.name "akilan" - Setting the name
 * git config --global user.email "akil.dove@gmail.com" - Setting the email
 * git config --global core.editor "gedit"
 * git config --global color.ui true
 * git config --list - It shows name & email
 * git config user.name - It shows akilan
 * All config values are located in /home/akilan/.gitconfig
 
# Git Basic Flow - Make Changes. Add Changes, Commit Changes

 * git init - creating .git folder to track the changes. It is invisible
 * ls -la .git/ - It maintain information about the project & repository
 * SVN puts a tracking file in every folder but GIT has only one folder to track all the changes
 * git add . - Add all the changes made in the entire project
 * git commit -m "Commit mesage" - Commits the changes with single line commit message
 * git status - to check the status of the project
 * git multiline commit message is a good practice & set a standard for a commit message
 * git log - Shows the recent log information
 * git log -n 5 - Last 5 commits
 * git log --since=01-01-2017 --until=01-12-2017 Lists the logs From jan 1, 2017
 * git log --grep="Ini" - Filter logs using regular expression
 * git log --author="akilan" - Filter logs by author name
 
# Git Architecture

 * Two tree Architecture - Repository & Working Copy
 * Three tree Architecture - Repository , Staging Index [ Add file before commit & then commit] & Working. Git uses thi
 s one
 * [Working Copy ] Create a  new file- Add the file [ git add Staging] - Commit changes [ Repository]
 * Each commits geneartes checksum 40 digit numebr to track. It is called commit id
 * HEAD points to the last commit id
