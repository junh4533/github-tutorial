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

Directory
Initialize - To prepare a repository for a certain language (in this case, Github language)
Repository (repo for short) - 

There are other terms that you should know. 
---
## Initial Setup

Step 1: Establishing the connection between Github and your coding platform (eg: Cloud 9, Nitrous, Codeacademy, etc..)

Before getting started, you have to understand that the cloud server where you store the files is known as the remote. 
In order to save the files online, you'll have to push it to the repo in the remote.
In most cases, the file will be pushed the remote nicknamed "origin".
Inside of origin, there are many brances. To keep things simple, you'll want to push it to the "master" branch in "origin".
The following code will establish a conection between your workspace and Github: git push -u origin master
Does it look familiar? Well, you already know what push, origin, and master means. 
The "-u" literally means upstream, which tells your computer to push it to the same place (origin master) everytime you push.
Next time you want to push code, you only have to type git push

Step 2: 

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
## Repository Setup




---
## Workflow & Commands