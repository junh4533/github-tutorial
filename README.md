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
To do that, 

go to settings in Github and 


---
## Repository Setup



---
## Workflow & Commands