# GitHub Tutorial

_by Nicholas Diaz_

---
## Git vs. GitHub
* What is _Git_ and how is it used?

**Git:** is used as a a tool for _version control_, like a snapshot, and works through the command line. Git **_does not need_** GitHub to work.

* What is _GitHub_?  

**GitHub:** is used to _collaborate_ with others, as well as visually track any changes made to your code and it's all stored on the cloud. GitHub also **_requires_** the use of git to work.

---
## Initial Setup

* First, create a [GitHub account](https://github.com) for use with Git.  

Linking your [Cloud9 account](https://c9.io) (can be signed in with GitHub) with your GitHub account requires the use of a **_Secure Shell_**, or **_SHH_** key, so information does not have to be included on a regular basis, and is always remembered.

1. Your SSH key can be found within the **settings** tab of Cloud9, _once signed in_ (Top Right, gear icon), and is in the menu to the left once inside titled "SSH Keys".
2. Once you've copyed the SSH key, return to your GitHub account and navigate to settings, **located once you've clicked your profile icon**. Once inside of settings, to the _left in the sidebar_, should be a tab titled "SSH keys".
3. Once inside this tab, there will be a button titled _"Add SSH key"_. Once clicked on, paste your SSH key into the box titled "key", and the title of the key should be Cloud9, or c9.io.
4. Next, time to set up your global username/email, for use in your IDE, which can be done with two commands, one being, git config --global user.name (Your first and last name goes here, without parenthesis), and git config --global user.email (Your email here)
5. After this step has been completed, in the console on the Cloud9 IDE and type "ssh -T git@github.com" (without quotes), and it will prompt you to say yes or no, type yes.
 * When this step is finished, you should get a message in your console saying, "Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access."


---
## Repository Setup
**Creating your first repository:**
 1. Creating a repository in Cloud9 must be **_spelled exactly the same way_** when created in GitHub (the remote), or it will not properly push.  
 2. The repository can be set up with the command "git init"  
   * `Important Side-note:`If you initialized git in the wrong directory, you'd have to remove git entirely from the directory by typing "rm -rf .git", this will completely remove git from the directory/repository.  
 3.Next, using an SSH key can be very beneficial to efficiency, as information does not have to be typed every time you want to add to a file through the console line. To always have a repository saved in where it is "pushed" to using a git command, which is shown when a new repository is first created in GitHub, shown here; git remote add origin git@github.com:(github username)/(repository name).git, (this allows you to push to your remote repository without having to type the whole URL) and git push -u origin master.  
4. Now, since your Cloud9 repository has been linked with it's remote counter-part, it can now be fully used, and added to from the Cloud9 IDE, using a set of git commands, such as add, commit, and push.


---
## Workflow & Commands

**Basics:** When working with Git and GitHub, it's important to learn the workflow of saving, adding, committing, and pushing to your remote repository.  
1. Saving your file after editing before starting your workflow process is the first step.  
2. After saving, you must **add** your file to the "stage", meaning it is ready to be committed (command: git add (filename).(extension)  
3. Next, is an optional command called "git status", which is used to check what files have been edited since the last commit.   
4. Commiting your file is the next step, using the command "git commit -m"(short but specific message)"". The reason for the message is for your own use, when looking back at past commits on GitHub so you have reference to what was changed in certain commits.  
5. Finally, the last command to use would be "git push", which will then "push" the code up to the remote repository.