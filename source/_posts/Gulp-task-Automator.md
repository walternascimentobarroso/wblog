title: Gulp task Automator
date: 2016-04-13 10:24:47
tags:
 - Front End
 - Development
---
The [Gulp](http://gulpjs.com/ "Official Site") came to help automate the tasks of developers Front End.

If you already work with front end development for some time already should be using various technologies such as Sass, live and reload etc., [gulp](http://gulpjs.com/ "Official Site") vei to put it all together in a only.
<!--more-->
There are others, but I like the gulp and I will focus on it
## Installation
First installed the [nodejs](/2016/04/01/Installing-nodejs/ "Installing nodejs"), then enter the command:
```
npm install -g gulp
```
After installation, we will start to use it
```
npm init
```
doing this way will create a file `package.json`, which will help in the project versioning, if you do not want to tell anything can go just pressing enter

## Modules
This is where the magic begins, you will put all the tasks you want to automate, example:
```
$ npm install browser-sync gulp --save-dev
```
Just one example of installation

After that simply create the `gulpfile.js`
```
var gulp        = require('gulp');
var browserSync = require('browser-sync').create();

gulp.task('browserSync', function () {
    browserSync({
        server: {
            baseDir: "src/"
        },
        options: {
            reloadDelay: 250
        },
        notify: false
    });
});
```
Just type `gulp browserSync` the terminal and ready is using browserSync with gulp.

## Using the harvest
There is many plugins to let the most powerful gulp if you want to take a look at the visit https://www.npmjs.com/ site I use some specific, however as I am lazy, I just found something wondrous the [Harvest](http://www.ryanbensonmedia.com/harvest "Official Site"), he already has everything ready (broserSync, sass, css minificador, javascript and images), just download or clone the project, then type:
```
$ npm install
```
then type in the terminal:
```
$ gulp
```
You will display a url for all features, if you have finished the project or want to publish type
```
$ gulp deploy
```
so you will create a folder with all files minicados ready for production

 > Obs .: when I started using gave a error to correct type `npm install --save-dev es6-promise` and in the `gulpfile.js` adicine `require('es6-promise').polyfill();` and can run pro hug

To have a better understanding you have to practice a lot with time you will create your own way to make your deployment and everything, but with this you will have a good starting point