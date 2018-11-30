# Github Tutorial
This document is a minimum tutorial of using git. It covers the most practical and fundamental usages of git, especially topics related to repositories and branches.

## Getting Started

### Prerequisites

There are several things that need to be done in advance:
1. Create an account at [GitHub](https://pages.github.com/)
2. Get a computer, Mac/Linux/Windows

## Set up your Git

You can set up your email address and username locally or globally, which means setting them up for a single repository or for every repository on your computer.

### Locally
1. Open Terminal.
2. Change the current working directory to the local repository where you want to configure the name that is associated with your Git commits.
3. Set your email address and username:
```
git config user.email "john.snow@example.com"
git config user.name "John Snow"
```
4. Confirm that you have set the Git username correctly:
```
git config user.email 
git config user.name
```

## Create a repository

A repository can be created in several ways:

### 1. Using GitHub

You can create a repository on GitHub following the simple creation instructions. Do not forget initializing your repository with a README.

### 2. From local files using cmd lines

More than often, you have developed some parts of a project before you realize that you want to put it on GitHub. Is it a little late? Don't worry. You can put your files on GitHub anytime you want.

Suppose you have a folder like this
```
/hello
    say_hello.py
```
Following the instructions below, you can create the repository you need.
1. [Generate a new SSH key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)
2. [Add it to you GitHub Account](https://help.github.com/articles/adding-a-new-gpg-key-to-your-github-account/)
3. Open terminal and change into the working directory
4. Initilize the local directory as a Git repository
```
$ git init
```
5. Add the files to your new local repository
```
$ git add .
```
6. Commit the files that you've staged in your local repository
```
$ git commit -m "Repository Created"
```
7. Create an empty repository on GitHub and copy the remote repository URL
8. In Terminal, add the URL for the remote repository where your local repository will be pushed
```
$ git remote add origin [paste copied URL here]
```
9. Push the changes in your local repository to GitHub
```
$ git push -u origin master
```
## Create/Delete a branch

### On GitHub

You can create or delete branches directly on GitHub, simply following the instructions.

### Create a new branch using cmd lines
1. Create the branch on your local machine and switch in this branch
```
$ git checkout -b [new_branch_name]
```
2. Push the branch on github :
```
$ git push origin [new_branch_name]
```

### Delete a branch using cmd lines
1. Delete a branch on your local filesystem (checkout first):
```
$ git branch -d [branch_name]
```
2. Delete the branch on github :
```
$ git push origin :[branch_name]
```

## Authors

* **Hong-Bo Deng** - *Initial work* - [Hong-Bo](https://github.com/Hong-Bo)
