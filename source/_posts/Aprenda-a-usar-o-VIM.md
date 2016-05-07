title: Aprenda a usar o VIM
date: 2016-04-10 09:50:46
tags:
 - vim
 - terminal
 - Development
---
O VIM é um VI melhorado, atualmente existem diversos editores de texto e IDEs de varios tipos, mas o VIM é um editor de texto que surgiu a varios anos e até hoje é um dos melhores.
<!--more-->
Por tanto se você quer melhoras suas habilidades de desenvolvimento, um bom editor de texto para isso é o vim, com ele você se tornará mais familiarido com o terminal e com o passar dos tempos se tornará algo produtivo até melhor que outras IDEs.

Para instalar o vim é muito simples, vá ate o terminal e digite:
```
sudo apt-get install vim
```
Para criar um arquivo ou editar digitem `vim` mais o nome do arquivo que deseja:
```
vim arquivo.c
```
> estou criando um arquivo .c, mas o vim pode ser utilizado em todos os tipos de arquivos com todos os tipos de extenções

## Comandos Básicos
Ao abrir um arquivo você inicia na tela de visualização, para entrar no modo de edição você precisa pressionar a tecla `i`.

No modo de edição você digita da forma que quiser, para copiar e colar voce pode fazer da mesma forma que faz no terminal, pressionando a sequencia de teclas `CTRL+SHIT+c` para copiar e `CTRL+SHIT+v` para colar.

Para copiar uma linha primeiro entre no modo de visualização, pressione a tecla `Esc` depois `:v`, com isso entrar no modo de visualização, agora para copiar uma linha, fique com o curso em cima dela e pressione `yy`, para colar, mova o curso até onde quer que seja colado e pressione a tecla `p`.

Para salvar o arquivo pressione a tecla `Esc` e depois `:w`.

Para fechar o arquivo pressione a tecla `Esc` e depois `:q`.

Para sair sem salvar o arquivo pressione a tecla `Esc` e depois `:q!`.

Para salvar e sair do arquivo em um unico comando pressione a tecla `Esc` e depois `:x`.

O vim possui diversos comandos esses são apenas o basico para começar.