---
layout: post
title: "Removing LAMP"
date: 2013-07-12 22:05
comments: true
categories: 
---
To remove the LAMP stack you may try the following commands.  
``` ruby Remove LAMP  
			$ sudo apt-get purge libapache2-mod-auth-mysql phpmyadmin
			$ sudo apt-get purge mysql-server mysql-server-5.1 mysql-server-core-5.1
			$ sudo apt-get purge apache2 apache2-mpm-prefork apache2-utils apache2.2-bin apache2.2-common libapache2-mod-php5
			$ sudo apt-get autoremove
```
