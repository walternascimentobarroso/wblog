title: Browser-sync a perfect livereload
date: 2016-04-05 11:34:56
tags:
- Development
- Front End
---
![Browsersync](https://www.browsersync.io/img/favicon.ico)

You that this used to create sites, at one point you be forced to test on multiple devices and screens of different sizes, ai test will test comes, finds an error in one device, open your favorite IDE and adjusts and around the forehead and realize that the pack on a screen broke in the other, now imagine if you had a tool that updated the page on all devices first connect.
<!--more-->
Well, that and the proposal of the [Browser-sync](https://www.browsersync.io/ "Official Site"), with it you can test on all devices at the same time and adjust the code to update it in every page, beautiful and magical: D
to install you need the [nodejs](/2016/04/01/Installing-nodejs/ "Installing nodejs")
```
npm install -g browser-sync
```
now that is installed, go to your project in the terminal and type
```
browser-sync start --server --files "css/*.css, *.html"
```
with that he will "listen" to all the changes in files with extensions html and css files inside the folder with extensions css

more information visit the [Official Site](https://www.browsersync.io/ "official Browser Sync-Site")