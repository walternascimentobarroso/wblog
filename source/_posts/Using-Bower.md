title: Using Bower
date: 2016-04-03 15:11:38
tags:
- Development
- Front End
---
![logo-nodejs](http://bower.io/apple-touch-icon.png)
Bower came to improve their lives, whenever we start a new project or we continue in an old, comes the dependancy, and it will have to go on site to site downloading all libraries want
<!-- more -->
But with the bower our problems are over
to install it you must first have the [nodejs](/2016/04/01/Installing-nodejs/ "Installing nodejs") installed, then just install the bower
```
npm install -g bower
```

so now we need to start the project
```
bower init
```
You will respond to a questionnaire and then will create a file named `bower.json`

this file (bower.json) is what u will send to your project and let the bower_components folder (you can change the name if you want) unversioned deminuindo project size

to install an dependecia u only need to put the package name
```
bower install <package>
```

if you have questions about the package name you can use the command
```
bower search <package>
```

but I still prefer the own site bower
```
http://bower.io/search/
```

whenever you start using a project or download and use it bower, you will need only enter
```
bower install
```

and be happy.