# Demo
I will write the important points here while learning more about git and github. 

## Creating Repository
Create a repository in the github, name it and then I have created readme.md in that repository named it "demo-repo".

## Setting SSH key
First of all I have opened Git Bash and gave these commands step by step
1. ssh-keygen -t ed25519 -C "saifullahsafi.official@gmail.com"
2. Then I entered three times and an SSH key was created 
3. Now adding the ssh key to the ssh--agent
4. Opened Powershell
5. entered this command [Get-Service -Name ssh-agent | Set-Service -StartupType Manual
Start-Service ssh-agent]
6. then entered this command [ssh-add c:/Users/islam/.ssh/id_ed25519]
7. after that using window file explorer C/Users/islam/.ssh I copied the passkey in  id_ed25519.pub.
8. Afterward, In the ssk key I added the key and gave it name ssh key

## VS code setup
Commands
1. git clone [ssh passkey] Used to clone the repository you want to work on in your local machine
2. changed the directory to the repo and made some changes.
3. git status (use to check if any changes were made)
4. git add . or git add [file name ] (used to stage all changes in the current or sub directory for the next commit, . is used for all you can also use file name instead)
5. git commit -m "some message" -m "some message" (used to commit changes -m is message used to enter some description for the commit, necessary).
6. git push origin main (used to upload your local commits to the remote repository's main branch on a platform like GitHub.)
7. Now you will be able to see changes made to the repository in github.

## making repository on local machine and then making it a github repo
1. create a folder
2. git init (to initialize git)
3. git add .
4. git commit
5. To make it suitable to be pushed and an origin is made for this repo we can do this [git remote add origin (ssn)]
6. to change branch from master to main [git branch main]
7. git push -u origin main (-u is used so that onward we just use git push instead of writing the whole thing).

## Feature Branch
1. To create feature branch into your existing code [git checkout -b BRANCHNAME]. 
2. Checkout command is used for changing branches while -b is used to create a new branch
3. If you commit the changes made, it will only be visible in the feature branch for now but if you change to main the changes won't be present there.
4. 
