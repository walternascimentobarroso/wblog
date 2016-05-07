title: Hexo to staticos blogs
date: 2016-04-07 09:48:24
tags:
 - Front End
 - tutorial
---
![Logo-hexo](https://hexo.io/icon/apple-touch-icon-114x114.png "Logo hexo")
The hexo is a new framework for creating static blogs, simple maintenance and super fast, and the description of the own [Official Site](https://hexo.io/ "hexo: Quick, simple and powerful") says: `The fast, simple & powerful blog framework`
<!--more-->
To use is necessary to have the [nodejs](/2016/04/01/Installing-nodejs/ "Installing nodejs") installed, then so is download and start using hexo
```
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```
Thus the hexo will already start a server on port 4000 and is only access the browser the link `http://localhost:4000/`

to create posts, you only have to type
```
hexo new "Title of the post or the name you want"
```
You will realize that created a new file with the name you put in the folder `source/_posts/`

To generate static files, so you should run the command
```
hexo generate
```
## Deploy
Now comes one of the coolest parts of hexo, with it you can export directly to the github pages (and elsewhere too), and to do this you only have to set the `_config.yml` file like this:
```
deploy:
  type: git
  repository: git@github.com:walternascimentobarroso/walternascimentobarroso.github.io.git
```
Switch to your repository ;)

## Own domain
And finally, if you already have a registered domain or want to use one, just create a `CNAME` file in the directory` source` and within the file put the url of your domain, example:
```
echo "walternascimento.com.br" > CNAME
```
Now the registry website br u will edit zone, and then add the type `A` and `192.30.252.153` address, then repeat the process and add the address, `192.30.252.154` and last mode the type to `CNAME` and put the url of your git repository pages `walternascimentobarroso.github.io` ready all in perfect condition.

For best references to access the [official website hexo](https://hexo.io/ "hexo: Quick, simple and powerful").