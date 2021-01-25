# what-is-git-github
basic git and github

1. create new branch (content-git-branch)
2. merge (content-git-branch) into main - create pull request

// FORK or FORKING is copy/duplicate other repository with their commit history into our own account(github account)

// DOWNLOAD or CLONE is download the zip file into our own computer

*******INSTALL GIT into windows**************
1. go to https://git-scm.com/ - download git for windows

Git command(local)
- $git init (make a normal empty folder to a git repo)
- $git add<file(s)> (add file into staging area where the file are ready to commit)
- $git status (check status of a file)
- $git commit
- $git config
- $git branch
- $git help

3 area in repo
- working tree (project folder)
- staging area (ready to commit)
- history        

example :
1. create new folder in desktop (ex: ina-test-repo)
2. open GIT BASH - go to folder ina-test-repo in desktop
                  how?
                  
                  1- $ pwd (print working directory- it shows current directory)
                     /c/User/ina
                     
                  2- $ls (-it will display all folders/files in the directory)
                  *remember we store ina-test-repo in desktop
                  
                  3- $ cd desktop (change directory to desktop)
                  currently we are on desktop directory
                  (to check - $ pwd)
                  /c/User/ina/desktop
                  
                  4- $ ls (is list)
                     desktop.ini ina-test-repo/
                     
                  5- $ cd ina-test-repo
                  currently we are on ina-test-repo folder
                  
                  ///make ina-test-repo to REPO GIT (master branch)///
                  
                  6- $ git init
                  Initialized empty Git repository in C:/Users/ina/Desktop/ina-test-repo/.git/
                  
                  we are currently on /desktop/ina-test-repo (master)
                  **create new html file in ina-test-repo - (ex: index.html)
                  7- $ git status 
                      On branch master

                      No commits yet

                      Untracked files:
                        (use "git add <file>..." to include in what will be committed)
                              index.html

                      nothing added to commit but untracked files present (use "git add" to track)

                  **add file to staging area
                  8- $ git add index.html
                  
                  9- $ git status
                      On branch master

                      No commits yet

                      Changes to be committed:
                        (use "git rm --cached <file>..." to unstage)
                              new file:   index.html

                  
