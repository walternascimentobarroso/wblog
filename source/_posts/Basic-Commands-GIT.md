title: Basic Commands GIT
date: 2016-04-12 09:57:09
tags:
 - GIT
 - Development
---
![Logo GIT](https://git-scm.com/images/logo@2x.png "Logo GIT")
## What is [GIT](https://git-scm.com "Official Site")?
[GIT](https://git-scm.com "Official Site") is a system of free distributed version control and open source, designed to handle everything from small to large projects with speed and efficiency, created in 2005 by Linus Torvalds. [Wikipedia](http://wikipedia.org/wiki/Git)
<!--more-->
The [GIT](https://git-scm.com "Official Site") is an optimal tool for work, and one of the main requirements for that are, or wish to join the area of development.

## What are the advantages?
Imagine being able to find changes in a project when they were made and who made ?, Imagine you can CTRL + Z throughout your project from the beginning, because that is what the [GIT](https://git-scm.com "Official Site") does.

The main advantage of git against other version control systems is their velociade and ability to work offiline.

[GIT](https://git-scm.com "Official Site") is currently one of the most discussed topics and is no shortage of tips and commands about it, therefore I will present only the most basic.

## Installation
To start if you are using Linux, possibly already must have [GIT](https://git-scm.com "Official Site") installed, if not, just type the following command:
```
sudo apt-get install git
```
o find the version installed in your just type `git --version`

## Setting up
### Configuring the terminal
to set the [GIT](https://git-scm.com "Official Site"), just type a few commands
```
$ git config --global color.status auto
$ git config --global color.branch auto
$ git config --global color.diff auto
$ git config --global color.ui always
$ git config --global core.editor vim
$ git config --global user.name "myname"
$ git config --global user.email "me@example.com"
```
Where have words quoted exchange for your name and email

### Setting the text editor
If you prefer you can use a text editor and find the .gitconfig file in your home folder, open and modify with text below:
```
[user]
    name = Name Lastname
    email = email@email.com
[ui]
    color = always
[color]
    ui = auto
    status = auto
    diff = auto
[core]
    editor = vim
```
Swapping `Name Lastname` and `email@email.com` by your name and email respectively.

after installation to start using the [GIT](https://git-scm.com "Official Site"), enough to type the command:
```
git init
```
With that you already have all the power of git

## Some commands
`git add <arquivo>` = add file
`git commit -s -m "[ACAO] Seu comentario"` = Creates a committee
`git fetch` = upgrading your base
`git push` = sends file to the repository
`git status` = shows the status
`git checkout` = restores the file to the version served
`git diff` = shows changes
`git rebase --continue` =  when any change in the first rebase
`git stash` = creates a temporary branch
`git blame <arquivo>` = see who made the change
`git  reset --soft HEAD~1` = Resets the last committee

## Graphical User Interfaces
`Gitk --all` = shows graphical area (`sudo apt-get install gitk`)
`Gitg --all` = shows graphical area (`sudo apt-get install gitg`)

## Extra
Finally, try to practice a lot because practice makes perfect and it is this link that it's great:
https://try.github.io/

Good studies.