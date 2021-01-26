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
- $git add . (add all edit/add files into staging area)
- $git status (check status of a file)
- $git commit -m (save file ex: git commit -m "Menambahkan file index.html)
- $git log (view all the commit history)/ ex: git log -- index.html (only for index.html) / ex: git log -3 (only 3 latest commit)
- $git checkout (to retrive back the deleted file, ex: $ git checkout 7272e -- style.css)
- $git config
- $git branch (add new branch, ex: add branch dosen and branch staff)
- $git log --all --decorate --oneline --graph (view network line of branches)
- $git help

#example modified mahasiswa.html
when we modified the file, we can add and commit simultaneously
example: $ git commit -am "menambah data pada file mahasiswa.html"

3 area in repo
- working tree (project folder)
- staging area (ready to commit)
- history        

example :
1. create new folder in desktop (ex: ina-test-repo)
2. open GIT BASH - go to folder ina-test-repo in desktop.
How?
                  
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
                  
3. make ina-test-repo to REPO GIT (master branch)
                  
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

4. add index.html file to staging area

                  8- $ git add index.html
                  
                  9- $ git status
                      On branch master

                      No commits yet

                      Changes to be committed:
                        (use "git rm --cached <file>..." to unstage)
                              new file:   index.html
                              
                  10- $ git commit -m "Menambahkan file index.html"
                      [master (root-commit) 2f5e603] Menambahkan file index.html
                       1 file changed, 12 insertions(+)
                       create mode 100644 index.html
                       
5. edit index.html file and add new file - style.css
                
                11- $ git status
                
                  On branch master
                  Changes not staged for commit:
                    (use "git add <file>..." to update what will be committed)
                    (use "git restore <file>..." to discard changes in working directory)
                          modified:   index.html

                  Untracked files:
                    (use "git add <file>..." to include in what will be committed)
                          style.css

                  no changes added to commit (use "git add" and/or "git commit -a")
                  
6. add all edit/add file into staging area
      
                12- $ git add .
                13- $ git status
                    On branch master
                    Changes to be committed:
                      (use "git restore --staged <file>..." to unstage)
                            modified:   index.html
                            new file:   style.css
7. commit all file in stage area

              14. $ git commit -m "edit file index.html and add style.css file
                  [master 7272ed9] edit file index.html and add style.css file
                   2 files changed, 7 insertions(+), 1 deletion(-)
                   create mode 100644 style.css
 
 8. to retrive deleted file (ex: style.css) - add 5 first #hash digit
 
              15. $ git checkout 7272e -- style.css
              16. $ git status
              
              On branch master
              Changes to be committed:
                (use "git restore --staged <file>..." to unstage)
                      new file:   style.css
                      
              17. $ git commit -m "retrive back style.css"
                  [master 0b3732f] retrive back style.css
                   1 file changed, 3 insertions(+)
                   create mode 100644 style.css
               
              18. $ git status
              
                  On branch master
                  nothing to commit, working tree clean
                  

              

              

              
