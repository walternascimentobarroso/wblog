title: Browser-sync um livereload perfeito
date: 2016-02-05 11:34:56
tags:
---
![Browsersync](https://www.browsersync.io/img/favicon.ico)

Você que esta acostumado a criar sites, em certo momento você se ver obrigado a testar em diversos dispositivos e telas de diferentes tamanhos, ai teste vai teste vem, encontra um erro em certo dispositivo, abre sua IDE favorita e ajusta e volta a testa e percebe que ao arrumar em uma tela quebrou na outra, imagine agora se você tivesse uma ferramenta que atualizasse a pagina em todos os dipositivos conectas.
<!--more-->
Pois é, essa e a proposta do [Browser-sync](https://www.browsersync.io/ "Site Oficial"), com ele você consegue testar em todos os dispositivos ao mesmo tempo e ao ajustar o codigo ele atualizar em todas as paginas, lindo e magico :D
para instalar você precisa do [nodejs](/2016/02/01/Instalando-NodeJs/ "Instalando NodeJs")
```
npm install -g browser-sync
```
agora que esta instalado, acesse seu projeto no terminal e digite
```
browser-sync start --server --files "css/*.css, *.html"
```
com isso ele irá "escutar" todas as mudanças ocorridas nos arquivos com extenções html e arquivos dentro da pasta css com extenções css

mais informações acesse o [Site Oficial](https://www.browsersync.io/ "Site oficial Browser-Sync")