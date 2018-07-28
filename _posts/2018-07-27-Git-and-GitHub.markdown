---
layout: post
title:  "Git and GitHub"
date:   2018-07-27 22:02:01 +0530
categories: Git
---

Notes for [Git Crash Course](https://www.youtube.com/watch?v=SWYqp7iY_Tc)

Version Control Systems(VCS)

VCS are used for tracking changes in computer files.  
	
Distributed version control systems

* Without having in same network.
* Remote repos like github and bitbucket.

Basic commands  

 ---

Initialize local git repository.  

	$ git init 

This will create a .git folder inside current folder.  

---
	
Add files to index.	
	
	$ git add <file>  

This will add files to the staging area(the area before you make commit)

---

Check status of working tree. 

	$ git status 

This will give you differences between the working tree and the staging area.  

---

commit changes in index and put it into local repository.

	$ git commit

---

Push to remote repositorylike github,bitbucket ,heroku  
	
	$ git push 
	
You can add SSH keys with github so that you dont have to add passwords.

---

Pull latest from remote repository.

	$ git pull

---

clone repository  into your current directory
	
	$ git clone

---
	
to remove a file added to staging area.

	$ git rm --cached <filename>

---

to add any files with .html extension
	
	$ git add *.html

---

to add every file to staging.
	
	$ git add .   

--

to add user credentials
	
	$ git config --global user.email "you@example.com"
	
	$ git config --global user.name "Your Name"

---

to commit changes
	
	$ git commit
	
a vim editor will pop up ,comment in this editor by removing the hash tag in the line.  
 Then press esc keytype  in the console below and  :wq to get out.By pass this editing stage using
 
 
 	$ git commit -m "<commit message>"

---

	 
Add .gitignore

Add a file named .gitignore  
Add files that you dont want to be staged include those files inside .gitignore file.Now when you add to staging area files in .gitignore will not be staged. Contents of .gitignore will look like this

	log.txt //for file
	/dir //for folder
	*.txt //for extensions
	
Branches

If a team of programmers are working on a project, one is building a login system. He can create a branch for that. He can commit changes to that branch without adding that to the master. When has done the project he can commit it to the master.

Create a branch.

	$ git branch <branch name>

Switch to branch Now you can do changes in the branch,when you are ready merge it to master.
	
	$ git checkout <branch name>

for merging a branch to master
	
	$ git merge <branch name> 

 Adding to remote repository
 get url from github.com
 You can find it under clone or download
 
 	$ git remote add origin https://github.com/Excelligence/sellervarsity-responsive.git
	$ git remote
	this will show our remote git repositories

push that to github

	$ git push origin master

after that for pushing only this command is required

	$ git push

clone other peoples repositories in full

	$ git clone <link>

to update changes other people have done to the repository.

	$ git pull
	
How to create a project folder and push it to GitHub
* Create project folder
* open git bash in this folder
* Initialize repo

  		$ git init

* Now stage files 

		$ git add .

* Commit changes

		$ git commit -m "message"
	
* Add to remote repo

		$  git remote add origin <url>
		
Here I think origin is the remote repo name in our local repository. In github the repo has  a separate name. If origin is already existing create origin2 or sth. Now remember to push exact repo name to github.

		$ git push -u origin master
		
Opening gitbash again in the same folder will allow us to continue were we left.
