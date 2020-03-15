# What Is Git ?

<img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/git-logo.png?raw=true" alt="Error"
	 width="550" />

 **Git** is a distributed revision control system that was made to be fast. Git was created by Linus Torvalds for use in developing the Linux kernel in 2005. Each working directory(project) using the Git version control system is a fully authorized _repository_ that includes whole modified files and version control system whitout central repo or no internet connetion.

Git design was inspired from BitKeeper and Monotone.
It is free and open source software released under the GNU General Public License version 2 software license.

---


## What is version control system ?
 
 **Version Control** is system that can saving and reverting to a specific version the one or more files that had modified. VCS is also referred to as _Revison Control_ and _Source Control_ system.
 
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

 <br/>

 **Installation control :**
 - ` git --verison  `
 
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
	 
 <br/>

To convert our index (folder) to Git project index :
 - ` git init  `	 

To see invisible git file : 
 - `ls -a` 
 
 <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_4.png?raw=true" alt="Error"
	 width="600" />

 <br/>

---



 ## Git Flowchart 
 
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/gitdiagram4.jpg?raw=true" alt="Error"
	 width="800" />
 
 <br/>
 
 To add a project files to Git Repository : 
 
 - `git add . or [file name] `

 Code `add` uses to send our project index to **Staging Area** from **Working Directory**. After that, to send the project to **Local Git Repo**, we need to `commit` it. 
 
 - `git commit -m " description "`
 
 
 
 <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_5.png?raw=true" alt="Error"
	 width="600" />

 <br/>
 
  To list the versions : 
 
 - `git log `

 <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_6.png?raw=true" alt="Error"
	 width="600" />

 <br/>

 > _I guess you realized the complicated hash code above, ı will mention about this subject in next title._
 
  To see situation of processes between Working Directory and Staging Area :
  
  - ` git status  `
  
  <img src=" https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_7.png?raw=true" alt="Error"
	 width="600" />
	 
 <br/>	 
 
  To see differs of changed files that are between Working Directory with Git Repo :
  
  - `git diff  [file name]  or . (dot) `

 <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_8.png?raw=true" alt="Error"
	 width="600" />
	 
 <br/>
 
  To see differs of changed files that are between Staging Area with Git Repo :
 
  - `git diff --staged ` 
  
  <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_9.png?raw=true" alt="Error"
	 width="600" />
 
  <br/>
  
  Code `git rm [file name]` uses for carrying file to Staging Area that had deleted in Working Directory. You don't have to add deleted file to Staging Area again. Code ` git rm -r [folder(index) name]` deletes index and included files.
  
    <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_10.png?raw=true" alt="Error"
	 width="600" />
	 
  <br/>
  
  Code `git mv [[file1 name] [file2 name] or a index]`  uses for carrying file to Staging Area that had renamed in Working Directory. You don't have to add renamed file to Staging Area again.
  
    <img src="https://github.com/barisdalyan/git-tutorial/blob/master/git/img/img_11.png?raw=true" alt="Error"
	 width="600" />
	 
  

  
  
	 
	 
 
