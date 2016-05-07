title: Um pouco de C faz bem
date: 2016-04-08 14:13:17
tags:
 - Development
 - Back End
---
A linguagem C é uma das mais utilizadas tanto em empresas como em faculdades, a linguagem C é uma linguagem tão poderosa que esta presente em diversos lugares, por esse motivo todos da area de TI deveriam conhecer pelo menos o básico da linguagem.
<!--more-->
Alguns sistemas linux ja vem um compilador de C instalado e algumas IDEs tornam a instalação bem simples, mas  se você estiver usando linux e não tiver instalado o gcc, basta seguir os comandos:
```
sudo apt-get update
```
isso vai atualizar sua lista e então você digita:
```
sudo apt-get install gcc
```
se com isso ainda não certo então digite:
```
sudo apt-get install build-essential
```
para criar algo em C é muito simples, e para mostrar como é simples vamos criar um programinha bem básico:
```
#include <stdio.h>

int main() {
	int a, b, c;
    a = 3;
    b = 5;
    c = a+b;
    printf("%d", c);
	return 0;
}
```
um programa bem simples que soma dois numeros em uma terceira variavel.
## Copilando
Agora vem a mágica, a copilação, salve o arquivo com o nome de `test.c` e então execute:
```
gcc test.c -o test
```
com isso você acaba de criar um programa chamado `test`, para executar o programa digite:
```
./test
```
após rodar o camando ele ira imprimir a variavel c.
## Biblioteca math.h
Existem varias operações simples que podemos fazer com o C, mas quando implementamos a biblioteca math.h, damos ao programa um poder a mais.

Com a biblioteca math podemos usar diversar funções ja prontas, um exemplo seria o código abaixo:
```
#include <stdio.h>
#include <math.h>

int main() {
	int a, b;
    a = 4;
    b = sqrt(a);
    printf("%d", b);
	return 0;
}
```
Agora vem a parte mais importante, quando for usar a biblioteca math.h, no momento de usar o comando para copilar, deve acrescentar o paramentro `-lm`, ficando assim:
```
gcc test.c -o test -lm
```
Última dica, se não quiser instalar na sua maquina ou estiver em um lugar onde não para instalar, tem um site otimo para fazer os teste, acessem:
https://ideone.com/

Pronto, sucesso, agora foco nos estudos