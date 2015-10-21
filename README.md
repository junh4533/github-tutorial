# GitHub Tutorial

_by Jun Huang_

---
## Git vs. GitHub
Git and Github is a platform that uses snapshots of your code to save it. 
You can revisit each change that is committed in order to go back to the previous working code. 
However, they're not exactly the same. The two lists below defines the differences between the two.

###Git:  
* Offline(local)  
* Doesn't require Github  

###Github:  
* Requires Git  
* Online(cloud-based) for collaboration  

In order to understand the basics of Git and Github, there are some terms thats you must know.

---
## Step 1: Initial Setup
This step will establish the connection between Github and your coding platform (eg: Cloud 9, Nitrous, Codeacademy, etc..)

Before establishing any connections, the first step is to make an account. Register for Github and your coding platform (if necessary).



Now the connection is established. But is it secure? The answer is NO. 
In order to make it secure, you'll have to set a SSH (secure shell) key that serves as a password for the connection. 
1. Go to the settings in your coding platform. There should be a tab about SSH keys. 
2. Navigate to that tab and copy the SSH key. 
3. In Github, go to settings and go into the SSH keys tab. 
4. Proceed to adding a SSH key. Be sure to give it a relevant title (the name of your coding platform is recommended)
5. Go back to your coding platform, into your IDE. Type in ssh -T git@github.com .Then type yes.

Congrats!! You have officially established a connection between your coding platform and Github. 
However, before you start coding, you still have to setup your repository.

---
## Step 2: Repository Setup
This step will initialize your repo and tells the computer where to save your files.

###Key Terms:
**_Directory_ - A folder that stores files**  
**_Initialize_ - To prepare a directory for a certain language (in this case, Github language)**  
**_Repository (repo for short)_ - An initialized repo, ready for coding**

To being coding, first you'll have to create a directory. Then initialize the directory so that it is a repo.

1. Make sure you're in the home folder.  
If you're in the home folder, you shouldn't be able to see any files when you type in `ls` into the IDE.
2. Make a directory using `mkdir (folder name)`.
3. Initialize the directory using `git init`.

Before you start coding, you would want a place where you can save your files online, in other words, the cloud. 
The cloud server where you store your files is known as the remote. 
In order to save the files online, you'll have to push it to the repo in the remote.
In most cases, the file will be pushed the remote nicknamed "origin".
Inside of origin, there are many branches. To keep things simple, you'll want to push it to the "master" branch in "origin".
The following code will establish a conection between your workspace and Github: `git push -u origin master`
Does it look familiar? Well, you already know what push, origin, and master means. 
The *"-u" literally means upstream*, which tells your computer to push it to the same place (origin master) everytime you push.
Next time you want to push code, you only have to type git push instead of typing the entire thing.

---
## Workflow & Commands
 
In order to upload your code to Github, you'll have to go through the process of saving, adding to stage, committing, and pushing.
*Key Terms* 
*Save - Storing a file locally*
*Add - Command to add a file to the stage*
*Stage - A place where a file is ready to be committed*
*Commit - Command to save a file locally on Git.*
*Push - Command to store files on Github*

The following steps will guide you into understanding the workflow of Github:

1. Save locally (you can find this option in the File Tab in the toolbar)
2. Add the file to the "stage" by typing `git add (file name)`. You can also add all files changed by typing `git add -all`. 
3. Commit the file by typing git commit -m "(message)".
The "-m" represents message and within the quotation marks that follows it,  
you can leave a message for yourself so you can go back and see what you've done in that save.
4. Push the file to the repo on Github by typing `git push`.