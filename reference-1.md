# Reference Day 1


1. Read at https://www.git-tower.com/learn/git/ebook/en/command-line/basics/what-is-version-control
2. Link source: https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-20-04
# Git installation on linux
Git is likely already installed in your Ubuntu 20.04 server. You can confirm this is the case on your server with the following command:

```git --version``` If you receive output similar to the following, then Git is already installed.

Output ```git version 2.25.1``` If this is the case for you, then you can move onto setting up Git, or you can read the next section on how to install from source if you need a more up-to-date version.

However, if you did not get output of a Git version number, you can install it with the Ubuntu default package manager APT.

First, use the apt package management tools to update your local package index.

sudo apt update With the update complete, you can install Git:

sudo apt install git You can confirm that you have installed Git correctly by running the following command and checking that you receive relevant output.

```git --version``` Output git version 2.25.1 With Git successfully installed, you can now move on to the Setting Up Git section of this tutorial to complete your setup.

Setting Up Git
After you are satisfied with your Git version, you should configure Git so that the generated commit messages you make will contain your correct information and support you as you build your software project.

Configuration can be achieved by using the git config command. Specifically, we need to provide our name and email address because Git embeds this information into each commit we do. We can go ahead and add this information by typing:

```git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"```
We can display all of the configuration items that have been set by typing:

```git config --list
Output
user.name=Your Name
user.email=youremail@domain.com
```

# Git installation on windows
https://gitforwindows.org/ or https://git-scm.com/download/win


Command used today:
mkdir test-git
cd test-git
git status
git init
echo "Hello text" > hello.txt
git add hello.txt
git commit -m "Initial commit"
git remote add origin https://github.com/vijaykchauhan/test-git.git
git branch -M main
git push -u origin main


