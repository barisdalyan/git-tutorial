**Author:**   [barisdalyan](https://github.com/barisdalyan)

---

# What Is Git ?

<img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/git-logo.png?raw=true" alt="Error"
	 width="550" />

 **Git** is a distributed revision control system that was made to be fast. Git was created by Linus Torvalds for use in developing the Linux kernel in 2005. Each working directory (project) using the Git version control system is a fully authorized _repository_ that includes whole modified files and version control system without central repo or no internet connetion.

Git design was inspired from BitKeeper and Monotone.
It is free and open source software released under the GNU General Public License version 2 software license.

---


## What is version control system ?
 
 **Version Control** is system that can saving and reverting to a specific version the one or more files that were modified. VCS is also referred to as _Revison Control_ and _Source Control_ system.
 
 You can handle over many issues using  Version Control System. 
 
These may be a problem for you ;
- Adding files in wrong index.
- Making a irrevocable writing mistake.
- Deleting files.
- You may want to know who made these mistakes. 
- And when was caused these mistakes. 

---

## Installation Git To Your System
> **Not:** _I'm going to tell mainly how to you use Git for Linux Operating System in this tutorial._

- You can reach Git site from [here.](https://git-scm.com/downloads)

<img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/git-site.png?raw=true" alt="Error"
	 width="550" />
	 
	 
	 
**Download for Linux :**
 
 - Debian/Ubuntu --> ` apt-get install git `
 - Arch Linux --> ` pacman -S git `
 
 
 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_1.png?raw=true" alt="Error"
	 width="600" />
	 
	 
	 

 <br>

 **Installation control :**
 
  - ` git --version  `
 
 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_2.png?raw=true" alt="Error"
	 width="600" />
	 
	 
	 
	 
 After installation, we need to configure our Git system.
  ```
  git config --global user.name " your name "
  git config --global user.email " your email address " 
  ```
  To checkout this configuration : 
 ```
 git config --global user.name 
 git config --global user.email 
 ```  
 
 
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_3.png?raw=true" alt="Error"
	 width="600" />
	 
	 
 <br>


To convert our index (folder) to Git project index :
 - ` git init  `	 

To see invisible git file : 
 
 - ` ls -a ` 
 
 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_4.png?raw=true" alt="Error"
	 width="600" />
	 


 <br>





 ## Git Flowchart 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/gitdiagram4.jpg?raw=true" alt="Error"
	 width="800" />
	 
 
 <br>
 
 To add a project file to Git Repository : 
 
  - `git add . or [file name] `

 We use command   `add`   to transfer our project index to **Staging Area** from **Working Directory**. After that, to transfer the project to **Local Git Repo**, we need to `commit` it. 
 
  - `  git commit -m " description "  `
 
 
 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_5.png?raw=true" alt="Error"
	 width="600" />



 <br>
 
  To list the versions : 
 
  - ` git log `




   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_6.png?raw=true" alt="Error"
	 width="600" />
	 
	 


 <br>

 > _I guess you realized the complicated hash code above, I will mention about this subject in next title._
 
  To see situation of processes between Working Directory and Staging Area :
  
  - ` git status  `
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_7.png?raw=true" alt="Error"
	 width="600" />
	 
	 
 <br>	 
 
  To see differs of changed files that are between Working Directory with Git Repo :
  
  - `git diff  [file name]  or . (dot) `
  

   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_8.png?raw=true" alt="Error"
	 width="600" />
	 
	 
 <br>
 
  To see differs of changed files that are between Staging Area with Git Repo :
 
  - `git diff --staged ` 
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_9.png?raw=true" alt="Error"
	 width="600" />
 
 
  <br>
  
  We use command   `git rm [file name]`   for carrying file, which was deleted in Working Directory, to Staging Area. You don't have to add deleted file to Staging Area again. Command   ` git rm -r [folder(index) name]`   deletes index and included files.
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_10.png?raw=true" alt="Error"
	 width="600" />
	 
	 
  <br>
  
  We use command   `git mv [[file1 name] [file2 name] or a index]`   for carrying file, which was renamed in Working Directory, to Staging Area. You don't have to add renamed file to Staging Area again.
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_11.png?raw=true" alt="Error"
	 width="600" />
	 
	 
  <br>
  
  ---
  
  To revert changes in file, which weren't   `added`   to Staging Area, in Working Directory :
  
  - `git checkout -- [file name] `
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_12%20(2).png?raw=true" alt="Error"
	 width="600" />
	 
	 
 <br>	 
  
  To revert changes in file which were  `added`  to Staging Area, in Working Directory :  
  
  - `git reset HEAD [file name]  `    but it has not reverted, yet. Write the code above again.
  
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_13.png?raw=true" alt="Error"
	 width="600" />
  
  
  
  <br>
  
  
  ## Changing Versions Between Each Other
  
  ```
  { version1 } -->{ version2 } -->{ version3 }
  ```
  
  İf we want to pass from [version3] to [version2] :
  
  -  `git checkout version2 [hash code of version] -- . `   (dot) or file name that we want to revert it to version2. 
  
  
  
  > **Not :** _You can write 6-7 digits hash code to blank side._
  
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_14.png?raw=true" alt="Error"
	 width="600" />
	 
  
  
  <br>
  
  
  
  
  ## How We Push Our Project to GitHub ?
  
  To connect with GitHub Repo : 
  
  - `  git remote add [nickname]  `   and   `  HTTPS address or SSH keyword  `
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/htpps.png?raw=true" alt="Error"
	 width="600" />
  
  
  
  
  To push the project :   
  
 - `  git push -u  `   (all files)   `  [nickname] master  `   After that, enter your GitHub email or nickname and password. That's all ! 
 
   
   
 <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_16.png?raw=true" alt="Error"
	 width="600" />
	 
  
  <br>
  
   To pull files from GitHub to your project index (folder) :
   
   - ` git pull`
  
  >  **Annotation :** _Git software must be integrated with your GitHub Repo._
  
  <br>
  
  
 ## Branches
 
 While you coding a program, seperating the project to branches is a wise way for division of labor. When each coworker completed their part of job, branches are merged by pull-request.
 
 - Command   ` git branch [new branch] `   creates new branch.
 
 - Command   ` git branch --all `   shows branches that belong to our GitHub Repo.
 
 To list available branches in Git system : 
 
 - `git branch`
 
 > Not : _`git branch -a `   shows branches that belong to our local Git Repository_
 
 
 
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_17.png?raw=true" alt="Error"
	 width="600" />
	 
 
 <br>
 
 To pass among branches, write this command to terminal :
  
  - `  git checkout [branch name]  `



   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_18.png?raw=true" alt="Error"
	 width="600" />
	
	
 <br>
 
  We should pass to master branch before merging branches with the master.
  Then  write this command to terminal : 
  
  
  - `  git merge [branch name]  `	
  
  
  
  
   <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_19.png?raw=true" alt="Error"
	 width="600" />
	 



 <br>
 
 
 By the way, we can see differs between master and new branch, through this command :
  - ` git diff master [new branch]  `
 
  > **Not:** _Square bracket " [ ] " was used for highlighting to instances._
  
  
  
	 
	 
 
