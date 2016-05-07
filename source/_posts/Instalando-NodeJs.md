title: Instalando NodeJs
date: 2016-04-01 15:24:33
tags:
- Development
---
![logo-nodejs](https://nodejs.org/static/apple-touch-icon.png)
Instalar  o node é bem fácil basta acessar o [site oficial](https://nodejs.org/en/ "Site oficial do nodejs") e baixar o pacote e pronto.
Mas se estiver com preguiça de clicar no link, você deve apenas digitar as linhas abaixo
<!-- more -->
```
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install -y nodejs
```
e para completar digite:
```
sudo apt-get install -y build-essential
```
veja se está tudo ok
```
node -v
```
pronto, node instalado com sucesso.
