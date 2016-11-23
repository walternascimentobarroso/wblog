title: Criando pendrive bootavel no Linux
date: 2016-11-22 23:11:38
tags:
- Linux
- Terminal
---
Dica Rapida e super util, de como instalar o linux em um pendrive deixando bootavel.
<!-- more -->
Existem varios programas graficos para criar o pendrive bootavel, mas a graça é usar um programa que ja vem por padrao no linux e usar no terminal.

```
$ sudo dd if=imagem_linux.iso of=/dev/onde_esta_o_pendrive
```

Para descobrir onde esta sua unidade do pendrive pode usar o comando

```
$ sudo fdisk -l
```

na maioria das vezes (pelo menos pra min) é /dev/sdb para ter certeza basta desconectar o pendrive e conectar denovo e ver o que muda, pronto agora que sabe qual a sua unidade use o comando dd

a tela ficara preta so com a seta piscando, vai demorar um pouco(muito dependendo da sua maquina) e pronto, pendrive bootavel criado ;)
