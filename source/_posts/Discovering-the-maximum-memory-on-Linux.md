title: Discovering the maximum memory on Linux
date: 2016-04-21 09:57:09
tags:
 - Linux
---
A few days ago I was to find out how much memory my notebook stand, despite being a simple command, I had to browse many sites to discover.
<!--more-->
I found diversar way and several new Linux commands, but will only show what really solved my problem

Open Terminal and type:
```
sudo dmidecode -t 16
```
will show various information
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
but if you want to know is the maximum memory is then only look where ta written `Maximum` to facilitate you can use the command:
```
sudo dmidecode -t 16 | grep Maximum
```
and it will show just what you are looking for.