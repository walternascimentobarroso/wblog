title: Descobrindo o máximo de memória no Linux
date: 2016-04-21 09:57:09
tags:
 - Linux
---
A alguns dias estive atras de descobrir quanto de memória meu notebook suportava, apesar de ser um comando simples, precisei navegar em muitos sites para descobri.
<!--more-->
Descobri diversar forma e varios novos comandos do linux, mas vou mostrar apenas o que realmente solucionou meu problema

Abra o terminal e digite:
```
sudo dmidecode -t 16
```
vai aparecer diversas informações
```
# dmidecode 2.12
SMBIOS 2.7 present.

Handle 0x0019, DMI type 16, 23 bytes
Physical Memory Array
	Location: System Board Or Motherboard
	Use: System Memory
	Error Correction Type: None
	Maximum Capacity: 32 GB
	Error Information Handle: No Error
	Number Of Devices: 2
```
mas se o que deseja saber é o máximo de memoria então é so olhar onde ta escrito `Maximum`, para facilitar você pode usar o comando:
```
sudo dmidecode -t 16 | grep Maximum
```
e com isso vai exibir apenas o que você procura.