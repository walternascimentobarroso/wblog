title: Comandos básicos do GIT
date: 2016-04-12 09:57:09
tags:
 - GIT
 - Development
---
![Logo GIT](https://git-scm.com/images/logo@2x.png "Logo GIT")
## O que é [GIT](https://git-scm.com "Site Oficial")?
[GIT](https://git-scm.com "Site Oficial") é um sistema de controle de versão distribuído livre e de código aberto, projetado para lidar com tudo, de pequenos a grandes projetos, com velocidade e eficiência, criado em 2005 por Linus Torvalds. [Wikipédia](http://pt.wikipedia.org/wiki/Git)
<!--more-->
O [GIT](https://git-scm.com "Site Oficial") é uma ferramenta otima para trabalho, e um dos principais requisitos para que é, ou deseja ingressar na area de desenvolvimento.
## Quais as vantagens?
Imagine poder descobrir alterações feitas em um projeto, quando foram feitas e quem fez?, Imagine você poder da CTRL+Z em todo seu projeto desde o inicio, pois é isso que o [GIT](https://git-scm.com "Site Oficial") faz.

A principal vantagem do git em relação a outros controles de versão é sua velociade e capacidade de poder trabalhar offiline.

[GIT](https://git-scm.com "Site Oficial") é atualmente um dos temas mais abordados e o que não falta são dicas e comandos sobre ele, por tanto vou apresentar so o mais basico.

## Instalação
Para começar se estiver usando o linux, possivelmente ja deve ter o [GIT](https://git-scm.com "Site Oficial") instalado, se não tiver, basta digite o comando abaixo:
```
sudo apt-get install git
```
para saber qual a versão instalada na maquina basta digitar `git --version`

## Configurando
### Configurando pelo terminal
para configurar o [GIT](https://git-scm.com "Site Oficial"), basta digitar alguns comandos
```
$ git config --global color.status auto
$ git config --global color.branch auto
$ git config --global color.diff auto
$ git config --global color.ui always
$ git config --global core.editor vim
$ git config --global user.name "meunome"
$ git config --global user.email "eu@example.com"
```
Onde tem palavras entre aspas troque pelo seu nome e seu email

### Configurando pelo editor de texto
Se preferir pode usar um editor de texto e  encontrar o arquivo .gitconfig na sua pasta home, abrir e modificar com texto abaixo:
```
[user]
    name = Nome Sobrenome
    email = email@email.com
[ui]
    color = always
[color]
    ui = auto
    status = auto
    diff = auto
[core]
    editor = vim
```
Trocando `Nome Sobrenome` e `email@email.com` por seu nome e email respectivamente.

após a instalação para comecar a utilizar o [GIT](https://git-scm.com "Site Oficial"), bastar digitar o comando:
```
git init
```
Com isso você ja terá todo o poder do git

## Alguns comandos
`git add <arquivo>` = adiciona o arquivo
`git commit -s -m "[ACAO] Seu comentario"` = Cria um comite
`git fetch` = atualizar sua base
`git push` = envia arquivo para o repositorio
`git status` = mostra os status
`git checkout` = restaura o arquivo pra versão do servido
`git diff` = mostra as alterações
`git rebase --continue` = quando ouver alguma mudança no primeiro rebase
`git stash` = cria um branch temporario
`git blame <arquivo>` = ver quem fez a alteração
`git  reset --soft HEAD~1` = Reseta o ultimo comite

## Interfaces Gráficas
`gitk --all` = mostra area grafica   (`sudo apt-get install gitk`)
`gitg --all` = mostra area grafica   (`sudo apt-get install gitg`)

## Extra
Para finalizar, tente praticar bastante pois a pratica leva a perfeição e para isso tem esse link que é otimo:
https://try.github.io/

Bons Estudos.