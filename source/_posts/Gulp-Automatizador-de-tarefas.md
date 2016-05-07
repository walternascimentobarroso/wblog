title: Gulp Automatizador de tarefas
date: 2016-04-13 10:24:47
tags:
 - Front End
 - Development
---
O [Gulp](http://gulpjs.com/ "Site Oficial") veio para ajudar a automatizar as tarefas de desenvolvedores Front End.

Se você ja trabalha com desenvolvimento front end a algum tempo ja deve estar usando diversas tecnologias como Sass, live reload e etc, o [gulp](http://gulpjs.com/ "Site Oficial") vei para juntar tudo isso em um só.
<!--more-->
Existem outros, mas gosto muito do gulp e vou focar nele
## Instalação
Primeiramente tenha instalado o [nodejs](/2016/04/01/Instalando-NodeJs/ "Instalando NodeJs"), então digite o comando:
```
npm install -g gulp
```
Após a instalação, vamos comecar a usa-lo
```
npm init
```
fazendo dessa forma será criado um arquivo `package.json`, que vai ajudar no versionamento do projeto, se não quiser informar nada pode ir apenas pressionando enter

## Módulos
Aqui é onde começa a magica, você vai colocar todas as tarefas que deseja automatizar, exemplo:
```
$ npm install browser-sync gulp --save-dev
```
Apenas um exemplo de instalação

Após isso basta criar o arquivo `gulpfile.js`
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
Com isso basta digitar `gulp browserSync` no terminal e pronto está usando o browserSync com o gulp.

## Usando o harvest
Existe diversos plugins para deixar o gulp mais poderoso se quiser da uma olhada acesse o site https://www.npmjs.com/ eu uso algumas especificas, porem como sou preguiçoso, acabei encontrado algo maravilho o [Harvest](http://www.ryanbensonmedia.com/harvest "Site Oficial"), ele ja tem tudo pronto (broserSync, sass, minificador de css, javascript e imagens), basta fazer o download ou clonar o projeto, depois digite
```
$ npm install
```
depois digite no terminal
```
$ gulp
```
com isso vai exibir uma url para com todas as funcionalidades, se tiver terminado o projeto ou quiser publicar digite
```
$ gulp deploy
```
assim você irá criar uma pasta com todos os arquivos minicados prontos para produção

 > Obs.: quando eu comecei a usar deu um error para corrigir digite `npm install --save-dev es6-promise` e no arquivo `gulpfile.js` adicine `require('es6-promise').polyfill();` e pode correr pro abraço

Para ter um melhor entendimento tem que praticar muito, com o tempo você irá criar sua propria forma de fazer seu deploy e tudo mais, porem com isso você tera um bom ponto de partida