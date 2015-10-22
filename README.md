# GitHub Tutorial

_by Ziqian Pan_

---
## Git vs. GitHub
**Git** is version control : that keeps snapshots of code, so if you need, you can look back at the previous version of your code and see what you did. You use use ```git init``` to start using Git's features on your local machine.

**GitHub** is a place where you store your code in the cloud and can colaborate with other coders really easiy by posting your code up in Github. You can make new repository that would connet to your local machine so you can push and pull any changes you have on the cloud.

**difference** Github is like the website and it can't run without Git, while Git can run on its own without GitHub and you use ```git init``` to start git in your currnet repository so you can start adding and commiting files.

---
## Initial Setup
**GitHub account** is needed before you can start using GitHub's features once you make the account then you can start making a repository and remotes to connet your local machine to your cloud. You can sign up for an account at [GitHub](https://github.com).  

**SSH key** is a very secure password that you can use to connet to two clients together so you can login safely. You have to go to your GitHub settings and within the settings you can find the SSH keys then you can click on add a SSH key and don't forget a title for the key as well. After that go back to the other client you are using (ex:Nitrous or c9) and find the SSH key on that client and copy and paste into GitHub now the two client that you are using is conneted.  

**Git config  (user.name & user.email)** ```git config user.name(name)``` are use to set up your name and ```git config user.email(email)``` is to set up your email address when you are using this repository and commiting it would send you a email and refer to you by your user.name. 

---
## Repository Setup
**Git init** is a code that will set up your repository so it can use all funtion of Git (**always remember to check where you are before using ```git init``` you have to be in the repository**) _so you don't enable git in the wrong repository._ When you want to enable git funtion in the repository you just type ```git init``` in the console of the repository that you want to enable **Git** in.

**First add and commit**, this will be the first time you ever in this fresh repository and you use ```git add <file name> ``` to add and you use ```git commit -m <message you want to see for this commit>``` to take a snapshot of your code so it would be in your revision history.

**New repository** can be made on GitHub, you have to first login to your github account then look to the top right where you will see a plus buttom. Click on that then click on Create new repository, then pick a Repository name(make sure it is the same as the repository you have on the other client(c9/Nitrous)) then click on Create repository. 

**remote** is a bridge you can setup so that you have a connetion between the two clients. You can do this by using the code < ```git remote add origin URL```>  

* you can get the URL from GitHub in the new repository that you just made, copy and paste the **SSH URL** over and put it in the URL section of the syntax.

After you setup your remote you are one step closer to make your first push. But first you have to setup where you are going to push to, and to do this you use```git push -u origin master``` since you named your remote connetion "origin" you are seting up so  that everytime you want to "```git push```" it will automatically push to the orgin (GitHub). Now you can ```git push``` freely, your setups are done


---
## Workflow & Commands
Normal workflow is 

1. you make/edit some code/files
2. use ```git status``` to check all recent modify files (use when you are not sure which file is on the stage)
3. use ```git add <file name>``` put the file on the stage to be commited
4. use ```git commit -m <"some info for this commit">``` takes a snapshot of your currnet code
5. lasty use ```git push``` to push all your new changes to GitHub where now everyone can see
6. repeat steps 1 -5