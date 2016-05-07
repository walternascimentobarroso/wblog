title: A bit of C is good
date: 2016-04-08 14:13:17
tags:
 - Development
 - Back End
---
The C language is one of the most used both in enterprises and colleges, the C language is a powerful language that is present in many places, for this reason all of the IT area should know at least the basics of the language.
<!--more-->
Some Linux systems already has an installed C compiler and some IDEs make simple installation, but if you are using Linux and you have not installed gcc, just follow the commands:
```
sudo apt-get update
```
this will update your list and then you type:
```
sudo apt-get install gcc
```
if still not sure then type:
```
sudo apt-get install build-essential
```
to create something in C is very simple, and to show how simple it is going to create a very basic little program:
```
#include <stdio.h>

int main() {
	int a, b, c;
    a = 3;
    b = 5;
    c = a+b;
    printf("%d", c);
	return 0;
}
```
a simple program that adds two numbers in a third variable.
## Compiling
Now comes the magic, the copilação, save the file with the name of `test.c` and then run:
```
gcc test.c -o test
```
with this you just created a so-called `test` program, to run the program type:
```
./test
```
after running camando it will print the variable c.
## Library math.h
There are several simple steps you can do with C, but when we implement the math.h library, give the program a more power.

With the math library can use diversar ready already functions, an example would be the code below:
```
#include <stdio.h>
#include <math.h>

int main() {
	int a, b;
    a = 4;
    b = sqrt(a);
    printf("%d", b);
	return 0;
}
```
Now comes the most important part, when using the math.h library when you use the command to copilar must add paramentro `-lm`, thus:
```
gcc test.c -o test -lm
```
Last tip, if you do not want to install on your machine or you are in a place where not to install, has a great site to do the test, access:
https://ideone.com/

Ready, success, now focus on studies