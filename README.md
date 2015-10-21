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

---
## Step 1: Initial Setup

_This step will establish the connection between Github and your coding platform (eg: Cloud 9, Nitrous, Codeacademy, etc..)_

Before establishing any connections, the first step is to make an account.  
Register for Github and your coding platform (if necessary).

Now the connection is established. But is it secure? The answer is NO.  
In order to make it secure, you'll have to set a SSH (secure shell) key that serves as a password for the connection.

1. Go to the settings in your coding platform. There should be a tab about SSH keys.  
2. Navigate to that tab and copy the SSH key.  
3. In Github, go to settings and go into the SSH keys tab.  
4. Proceed to adding a SSH key. Be sure to give it a relevant title (the name of your coding platform is recommended).  
5. Go back to your coding platform, into your IDE. Type in ssh -T git@github.com .Then type yes.

Congrats!! You have officially established a connection between your coding platform and Github. 
However, before you start coding, you still have to setup your repository.

---
## Step 2: Repository Setup

_This step will initialize your repo and tells the computer where to save your files._

###Key Terms:
**_Directory_ - A folder that stores files**  
**_Initialize_ - To prepare a directory for a certain language (in this case, Github language)**  
**_Repository (repo for short)_ - An initialized repo, ready for coding**
**Save - Storing a file locally**  
**Add - Command to add a file to the stage**  
**Stage - A place where a file is ready to be committed**  
**Commit - Command to save a file locally on Git.**

To being coding, first you'll have to create a directory. Then initialize the directory so that it is a repo.

1. Make sure you're in the home folder.  
If you're in the home folder, you shouldn't be able to see any files when you type in `ls` into the IDE.
2. Make a directory using `mkdir (folder name)`.
3. Initialize the directory using `git init`.

Let's test out your first repo!  
To do so, let's make a file inside your repo using `touch (file name)`.
Make sure you're in the folder where you want to create the file. 
If you make in the wrong folder, you can always use `rm (file name)` to delete the file.

Now you'll have to login and configure your account.
The following code will log you into Github in your coding platform.  
**The global means that this will apply for all repositories and the "--" remembers that you have logged in and so this is a one time setup.**

`git config --global user.name (name)`  
`git config --global user.email (email)`

Now let GIT started on your test repo.

1. Edit the file that you created. Type anything you want into the file.
2. Make sure you're inside of the folder that contains the file.  
3. Type `git add (file name)` in the IDE.
4. Type `git commit -m "(message)"`.

You've finished making the repo on your coding platform. 
But you also need a repo on Github. To do so, follow the next steps.

1. Go to Github and click on the + symbol on the toolbar.
2. Select new repo.
3. Name the repo **EXACTLY THE SAME AS THE ONE IN YOUR CODING PLATFORM**.
4. Create the repo and make sure SSH is selected.

_next section of the tutorial will explain the workflow of the commands that you just used._
_Don't be too worried about not understanding it._

---
## Workflow & Commands

In order to upload your code to Github, you'll have to go through the process of saving, adding to stage, committing, and pushing.

**Key Terms:**  
**Push - Command to send files from your local machine to the Github repo**


The following steps will guide you into understanding the workflow of Github:

***Once in a while, you might want to use `git status` to see if the files are added to the stage.** 
**You can also use it to see if your files have been committed.**

1. Save locally (you can find this option in the File Tab in the toolbar)  
2. Add the file to the "stage" by typing `git add (file name)`. You can also add all files changed by typing `git add -all`.  
3. Commit the file by typing git commit -m "(message)".  
The "-m" represents message and within the quotation marks that follows it,  
you can leave a message for yourself so you can go back and see what you've done in that save.  

Now you would want to push the files to Github.
The cloud server where you store your files is known as the remote.  
In order to save the files online, you'll have to push it to the repo in the remote.  
In most cases, the file will be pushed the remote nicknamed "origin".  
Inside of origin, there are many branches. To keep things simple, you'll want to push it to the "master" branch in "origin".  

4. Type `git push -u origin master`.  
Does it look familiar? Well, you already know what push, origin, and master means.  
The **"-u" literally means upstream**, which tells your computer to push it to the same place (origin master) everytime you push.  
Next time you want to push code, you only have to type git push instead of typing the entire thing.
