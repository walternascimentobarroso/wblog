title: Brincando com o Angular Material
date: 2016-04-14 10:09:39
tags:
 - Front End
 - Development
---
[Angular Material](https://material.angularjs.org/) é uma implementação da referência do Google material, é um projeto com diversos componentes testados e prontos para uso.
<!--more-->
Indo direto ao assunto, para começar você pode criar uma pagina `index.html`, com o seguinte conteudo (Copiado do site do [Angular Material](https://material.angularjs.org/)):
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
Nesse caso está sendo utilizado tudo via CDN do google, mas se você quiser poderá usar o  [bower](/2016/04/03/Usando-Bower/ "Usando o Bower") para baixar todas as dependencias

Após isso basta você acessar o site do [angular material](https://material.angularjs.org/) na parte de demos e usar o exemplo que quiser, é uma ferramenta bem simples e para usar é necessario poucas linhas de codigos, qualquer duvida veja a documentação