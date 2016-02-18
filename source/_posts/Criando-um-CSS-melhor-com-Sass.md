title: Criando um CSS melhor com Sass
date: 2016-02-04 09:44:53
tags:
---
Escrever CSS é algo simples e fácil, principalmente no começo de qualquer projeto, mas conforme os dias vão passando as linhas de códigos aumentando fica cada vez mais dificil organizar o código css, e para facilitar nossa vida surgiu os pré-processadores
<!--more-->
Existem diversos pré-processadores, mas vou falar do mais utilizado e o qual estou trabalhando atualmente, o [Sass](http://sass-lang.com/ "Site oficial do Sass")
Você escrevendo css ja deve ter varias vezes copiado e colado varias linhas, ou ja deve ter imaginado varias como como seria bom ter varias no css pelo menos para salvar aquela cor principal do sistema, e o [Sass](http://sass-lang.com/ "Site oficial do Sass") tem tudo isso.
para instalar não tem segredo, apenas digite
```
sudo su -c "gem install sass"
```
qualquer dúvida acesse o [Site Oficial](http://sass-lang.com/install "Site oficial do Sass")
para saber se instalou corretamente digite
```
sass -v
```
deve retornar algo como 
`Sass 3.4.21 (Selective Steve)`
agora que esta instalado, vem a parte divertido(criar codigo)
agora quando você for criar um arquivo css, você nao ira mais utilizar a extenção .css, agora irá utilizar a extenção .scss e o proprio [Sass](http://sass-lang.com/ "Site oficial do Sass") se encarregarar de criar o css para você
abra um terminal separado e digite
```
sass --watch style.scss:style.css
```
com isso o [Sass](http://sass-lang.com/ "Site oficial do Sass") vai ficar sempre 'escutando' o arquivo style.scss, e qualquer modificação ele ira compilar para o style.css
Uma das maiores vantagens é a crianção de variaveis, veja um exemplo
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
e agora quando precisar mudar a cor so precisa mudar em um unico lugar
Outra grande vatangem é o uso de mixin, com ele você escreve algo comun para muitos (tipo uma classe) e depois aplica onde quer usar as linhas repetidas(tipo herança)
exemplo:
```
    @mixin common {
        color: blue;
        float: left;
    }
    #menu { @include common; }
    #main { @include common; }
```
muito util e muito facil de usar, se você ainda não utiliza, então comece agora mesmo.
para mais funcionalidades acesse o  [Site Oficial](http://sass-lang.com/install "Site oficial do Sass")