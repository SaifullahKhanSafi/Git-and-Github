# Demo
I will write the important points here while learning more about git and github. 
________________________________________________________________________________________________________________

## Creating Repository
Create a repository in the github, name it and then I have created readme.md in that repository named it "demo-repo".
________________________________________________________________________________________________________________
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
________________________________________________________________________________________________________________
## VS code setup
Commands
1. git clone [ssh passkey] Used to clone the repository you want to work on in your local machine
2. changed the directory to the repo and made some changes.
3. git status (use to check if any changes were made)
4. git add . or git add [file name ] (used to stage all changes in the current or sub directory for the next commit, . is used for all you can also use file name instead)
5. git commit -m "some message" -m "some message" (used to commit changes -m is message used to enter some description for the commit, necessary).
6. git push origin main (used to upload your local commits to the remote repository's main branch on a platform like GitHub.)
7. Now you will be able to see changes made to the repository in github.
________________________________________________________________________________________________________________
## making repository on local machine and then making it a github repo
1. create a folder
2. git init (to initialize git)
3. git add .
4. git commit
5. To make it suitable to be pushed and an origin is made for this repo we can do this [git remote add origin (ssn)]
6. to change branch from master to main [git branch main]
7. git push -u origin main (-u is used so that onward we just use git push instead of writing the whole thing).
________________________________________________________________________________________________________________
## Feature Branch
1. To create feature branch into your existing code [git checkout -b BRANCHNAME]. 
2. Checkout command is used for changing branches while -b is used to create a new branch
3. If you commit the changes made, it will only be visible in the feature branch for now but if you change to main the changes won't be present there.
4. Checkout to main branch and use diff command to view all the difference between feature and main branch
[git diff FEATURENAME]
5. after commiting psh the changes on the feature branch as push request for the main using (git push -u origin FEATURENAME).
6. after that check for the pull requests in the github repo and merge the pull request with the main code if approved.
7. After approving the pull request you have to pull the code to your local machine using (git push origin main).
8. To delete a approved feature branch (git branch -d BRANCHNAME).
_______________________________________________________________________________________________________________

1. Hello
2. Hi
________________________________________________________________________________________________________________
## Undoing git changes
1. to undo any git changes you can use git reset.
2. But if you have committed accidently than that commit is stages but what if you want to go back you can use (git rest HEAD~1). Basically this tells git that HEAD which is a pointer that points to commits it tell them using telda to go back one commit from the current.
3. (git log ) to check for all the logs of commits made.
4. (git reset --hard [logaddress]) to not just unstage the commit but also remove all the changes made.
________________________________________________________________________________________________________________
