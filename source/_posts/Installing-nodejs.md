title: Installing nodejs
date: 2016-04-01 15:24:33
tags:
- Development
---
![logo-nodejs](https://nodejs.org/static/apple-touch-icon.png)
Installing the node is easy enough to access the [official website](https://nodejs.org/en/ "Official Site nodejs") and download the package and ready.
But if you are too lazy to click the link, you should just enter the following lines
<!-- more -->
```
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install -y nodejs
```
and to complete type:
```
sudo apt-get install -y build-essential
```
see if everything is ok
```
node -v
```
ready, node successfully installed.
