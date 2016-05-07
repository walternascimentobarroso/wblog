title: Transferring file with SCP
date: 2016-04-17 09:29:49
tags:
 - Development
---
When using ssh able to connect to a machine and do everything like we had in front of her, but there comes a time that we want to copy something from the machine that we are for the remote machine or vice versa, and at that time enters the [SCP](https://wikipedia.org/wiki/Unix_SCP "Wikipedia").
<!--more-->
If we are in our machine and we have to send a file simply type the following command:
```
$ scp /home/usuario/texto.txt servidor@192.168.0.1:/home/servidor
```
Thus the `texto.txt` file will be copied to the machine` 192.168.0.1` in the directory `/home/servidor`.

To retrace just type the following command:
```
$ scp servidor@192.168.0.1:/home/servidor/texto.txt /home/usuario/
```
Thus the `texto.txt` file is copied to the local machine in the directory `/home/usuario`.

For more information about the type command:
```
$ man scp
```