title: Usando Bower
date: 2016-02-03 15:11:38
tags:
---
![logo-nodejs](http://bower.io/apple-touch-icon.png)
Bower veio para melhorar sua vida, sempre que iniciamos um projeto novo ou damos continuidade em um antigo, vem as dependecias, e la vai ter que ir de site em site baixando todas as bibliotecas que queremos
<!-- more -->
Mas com o bower nossos problemas acabaram
para instala-lo primeiro você deve ter o  [nodejs](/2016/02/01/Instalando-NodeJs/") instalado, depois é só instalar o bower
```
npm install -g bower
```

agora so precisamos iniciar o projeto
```
bower init
```
Você ira responder um questionario e depois será criado um arquivo com o nome `bower.json`

esse arquivo (bower.json) é o que vc ira enviar para seu projeto e deixar a pasta bower_components (que você poderar mudar  o nome se quiser) não versionada deminuindo o tamanho do projeto

para instalar uma dependecia vc so precisa colocar o nome do pacote
```
bower install <package>
```

se tiver duvidas sobre o nome do pacote você pode usar o comando
```
bower search <package>
```

mas eu ainda prefiro pelo proprio site do bower
```
http://bower.io/search/
```

sempre que for começar usar um projeto ou baixar e ele usar o bower, você só precisara digitar
```
bower install
```

e seja feliz.