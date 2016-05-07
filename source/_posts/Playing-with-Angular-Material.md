title: Playing with Angular Material
date: 2016-04-14 10:09:39
tags:
 - Front End
 - Development
---
[Angular Material](https://material.angularjs.org/) is an implementation of Google reference material, is a project with many tested and ready to use components.
<!--more-->
Going straight to the point to begin with you can create a page `index.html`, with the following content (site Copied from [Angular Material](https://material.angularjs.org/)):
```
<html lang="en" >
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- Angular Material style sheet -->
  <link rel="stylesheet" href="http://ajax.googleapis.com/ajax/libs/angular_material/1.0.0/angular-material.min.css">
</head>
<body ng-app="BlankApp" ng-cloak>
  <!--
    Your HTML content here
  -->  
  
  <!-- Angular Material requires Angular.js Libraries -->
  <script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular.min.js"></script>
  <script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular-animate.min.js"></script>
  <script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular-aria.min.js"></script>
  <script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular-messages.min.js"></script>

  <!-- Angular Material Library -->
  <script src="http://ajax.googleapis.com/ajax/libs/angular_material/1.0.0/angular-material.min.js"></script>
  
  <!-- Your application bootstrap  -->
  <script type="text/javascript">    
    /**
     * You must include the dependency on 'ngMaterial' 
     */
    angular.module('BlankApp', ['ngMaterial']);
  </script>
  
</body>
</html>
```
In this case it is being used all CDN via google, but if you want you can use the [Bower](/2016/04/03/Using-Bower/ "Using Bower") to download all dependencies

After that you can simply access the site [angular materials](https://material.angularjs.org/) on the demos and use the example you want is a simple tool to use and is necessary few lines of codes, no doubt see the documentation