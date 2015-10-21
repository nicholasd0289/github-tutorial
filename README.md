# GitHub Tutorial

_by Nicholas Diaz_

---
## Git vs. GitHub
* What is _git_ and how is it used?

**Git:** is used as a a tool for _version control_, like a snapshot, and works through the command line. Git **_does not need_** GitHub to work.

* What is _GitHub_?  

**GitHub:** is used to _collaborate_ with others, as well as visually track any changes made to your code and it's all stored on the cloud. GitHub also **_requires_** the use of git to work.

---
## Initial Setup

* First, create a [GitHub account](https://github.com) for use with Git.  
 1. Creating a repository in Cloud9 must have the same wording when created in GitHub, or it will not properly push.
 2. The repository can be set up with the command "git init"
   * `Important Side-note:`If you initialized git in the wrong directory, you'd have to remove git entirely from the directory by typing "rm -rf .git", this will completely remove git from the directory/repository.
 3. Once this is done, in the console line in the Cloud9 IDE, to set up your 

Linking your [Cloud9 account](https://c9.io) (can be signed in with GitHub) with your GitHub account requires the use of a **_Secure Shell_**, or **_SHH_** key, so information does not have to be included on a regular basis, and is always remembered.

1. Your SSH key can be found within the **settings** tab of Cloud9, _once signed in_ (Top Right, gear icon), and is in the menu to the left once inside titled "SSH Keys".
2. Once you've copyed the SSH key, return to your GitHub account and navigate to settings, **located once you've clicked your profile icon**. Once inside of settings, to the _left in the sidebar_, should be a tab titled "SSH keys".
3. Once inside this tab, there will be a button titled _"Add SSH key"_. Once clicked on, paste your SSH key into the box titled "key", and the title of the key should be Cloud9, or c9.io.
4. After this step has been completed, in the console on the Cloud9 IDE and type "ssh -T git@github.com" (without quotes), and it will prompt you to say yes or no, type yes.
 * When this step is finished, you should get a message in your console saying,

---
## Repository Setup



---
## Workflow & Commands