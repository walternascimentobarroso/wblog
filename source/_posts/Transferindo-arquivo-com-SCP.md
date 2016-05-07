title: Transferindo arquivo com SCP
date: 2016-04-17 09:29:49
tags:
 - Development
---
Ao utilizar o ssh conseguimos nos conectar em uma maquina e fazer tudo como se tivéssemos em frente dela, mas chega um momento que queremos copiar algo da maquina que estamos para a maquina remota ou vice-versa, e nesse momento entra o [SCP](https://pt.wikipedia.org/wiki/Unix_SCP "Wikipédia").
<!--more-->
Se estamos em nossa maquina e temos que enviar um arquivo basta digitar o comando abaixo:
```
$ scp /home/usuario/texto.txt servidor@192.168.0.1:/home/servidor
```
Com isso o arquivo `texto.txt` será copiado para a maquina `192.168.0.1` no diretorio `/home/servidor`.

Para fazer o inverso basta digita o comando abaixo:
```
$ scp servidor@192.168.0.1:/home/servidor/texto.txt /home/usuario/
```
Com isso o arquivo `texto.txt` será copiado para a maquina local no diretorio `/home/usuario`.

Para mais informações sobre o comando digite:
```
$ man scp
```