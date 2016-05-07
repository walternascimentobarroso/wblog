title: Learn how to use VIM
date: 2016-04-10 09:50:46
tags:
 - vim
 - terminal
 - Development
---
VIM is an improved VI, currently there are many text editors and IDEs of various types, but the VIM is a text editor that arose several years and is still one of the best.
<!--more-->
Therefore if you want improvements your development skills, a good text editor for this is vim, with it you will become more familiarido with the terminal and with the passage of time will become something productive even better than other IDEs.

To install vim is very simple, go up the terminal and type:
```
sudo apt-get install vim
```
To create a file or edit to type `vim` more the name of the file you want:
```
vim arquivo.c
```
> I'm creating a .c file, but vim can be used in all types of files with all types of extensions

## Basic Commands
When you open a file you start in the preview screen to enter the edit mode you must press the `I` key.

In edit mode you type the way you want to copy and paste you can do the same way it does in the terminal by pressing the sequence of keys `Ctrl + SHIT + c` to copy and `CTRL + SHIT + V` to paste .

To copy a line between the first display mode, press the key after Esc`:v`, thereby entering the viewing mode, now to copy a line, keep the course on top of it and press `yy`, to paste, move the course to wherever it is glued and press the `p` key.

To save the file press the `Esc` key and then: `w`.

To close the file press the `Esc` key and then: `q`.

To exit without saving the file press the `Esc` key and then: `q!`.

To save and exit the file in a single command press the `Esc` key and then: `x`.

Vim has many commands those are just the basics to get started.