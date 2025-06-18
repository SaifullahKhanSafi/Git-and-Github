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