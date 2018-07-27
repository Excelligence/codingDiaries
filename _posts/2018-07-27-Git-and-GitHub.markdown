---
layout: post
title:  "Git and GitHub"
date:   2018-07-27 22:02:01 +0530
categories: Git
---

https://www.youtube.com/watch?v=SWYqp7iY_TcVersion Control Systems
	* for tracking changes in computer files.  
	


	Distributed version control systems
	* Without having in same network.


	* Remote repos like github and bitbucket

Basic commands  
  
	$ git init //initialize local git repositoryThis will create a .git folder in that project.  
	
	$ git add <file> //Add files to index.This will add files to the staging area(the area before you make commit)   


	$ git status //Check status of working treeThis will give you differences between the working tree and the staging area.  
	
	$ git commit //commit changes in index and put it into local repository.$ git push // Push to remote repositorylike github,bitbucket ,herokuYou can add SSH keys with github so that you dont have to add passwords.$ git pull // Pull latest from remote repository.$ git clone // clone repository  into your current directory.$ git rm --cached <filename> // to remove a file added to staging area.$ git add *.html // to add any files with .html extension$ git add .   // to add every file to staging.$ git config --global user.email "you@example.com"$ git config --global user.name "Your Name"When enter $ git commita vim editor will pop upcomment in this editor by removing the hash tag in the line. Then press esc keytype  in the console below :wq to get outBy pass this editing stage using$ git commit -m "<commit message>"Add .gitignoreAdd a file named .gitignoreAdd files that you dont want to include in inside that.Now when you add to staging area files in .gitignore will not be staged.contents of .gitignore will look like thislog.txt //for file/dir //for folder*.txt //for extensionsBranchesIf a team of programmers are working on a project, one is building a login system. He can create a branch for that. He can commit changes to that branch without adding that to the master. When has done the project he can commit it to the master.$ git branch <branch name>Create a branch.$ git checkout <branch name>Switch to branch Now you can do changes in the branch,when you are ready merge it to master.$ git merge <branch name> //for merging a branch to master Adding to remote repositoryget url from github.comYou can find it under clone or download$ git remote add origin https://github.com/Excelligence/sellervarsity-responsive.git$ git remotethis will show our remote git repositories$ git push origin masterpush that to github$ git pushafter that for pushing only this command is required$ git clone <link>clone other peoples repositories in full$ git pullto update changes other people have done to the repository.How to create a project folder and push it to GitHub
	* Create project folder
	* open git bash in this folder
	* Initialize repo

        $ git init
	* Now stage files 

$ git add .
	* Commit changes

$ git commit -m "message"
	* Add to remote repo

$  git remote add origin <url>Here I think origin is the remote repo name in our local repository. In github the repo has  a separate name. If origin is already existing create origin2 or sth. Now remember to push exact repo name to github.$ git push -u origin masterOpening gitbash again in the same folder will allow us to continue were we left.
