title: Creating a CSS better with Sass
date: 2016-04-04 09:44:53
tags:
- Development
- Front End
---
Write CSS is something simple and easy, especially at the beginning of any project, but as the days go by the lines of code increasing becomes increasingly difficult to organize CSS code, and to facilitate our lives pre-processors came
<!--more-->
There are several pre-processors, but I will talk about the most used and which I am currently working on the [Sass](http://sass-lang.com/ "Official Site Sass")
You must have already writing css several times copied and pasted several lines, or already should have known several like it would be nice to have several in css at least to save her main color system, and [Sass](http://sass-lang.com/ "official Site Sass") has it all.
install to have no secret, just type
```
sudo su -c "gem install sass"
```
no doubt go to the [Official Site](http://sass-lang.com/install "Official Site Sass")
to see if installed correctly type
```
sass -v
```
should return something like
`Sass 3.4.21 (Selective Steve)`
now that is installed comes the fun part (create code)
Now when you are creating a CSS file, you will not longer use the .css extension, will now use the .scss extension and own [Sass](http://sass-lang.com/ "official Sass Site") if encarregarar to create the CSS for you
open a separate terminal and type
```
sass --watch style.scss:style.css
```
thus the [Sass](http://sass-lang.com/ "Official Site Sass") will always be 'listening' style.scss the file, and any changes it will compile to style.css
One of the biggest advantages is the big kid of variables, see an example
```
    $color: #c0c0c0
     
    .window-teste{
       background: $color;
    }
    .button-teste{
       background: $color;
    }
    .link-teste{
       background: $color;
    }
```
and now when you need to change the color so you need to change in a single place
Another great vatangem is the use of mixin with it you write something comun to many (like a class) and then applies wherever use repeated lines (type inheritance)
example:
```
    @mixin common {
        color: blue;
        float: left;
    }
    #menu { @include common; }
    #main { @include common; }
```
very useful and very easy to use, if you do not use, so start right now.
for more features visit the [Official Site](http://sass-lang.com/install "Official Site Sass")