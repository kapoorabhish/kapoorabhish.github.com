---
layout: post
title: "Installing phpMyAdmin"
date: 2013-07-08 22:29
comments: true
categories: 
---
Here I am going to post some steps in order to install phpMyAdmin.  
{% codeblock %}
sudo apt-get install phpmyadmin
{% endcodeblock %}

Once the process starts up, follow these steps:  
* Select Apache2 for the server  
* Choose YES when asked about whether to Configure the database for phpmyadmin with dbconfig-common  
* Enter your MySQL password when prompted  
* Enter the password that you want to use to log into phpmyadmin  


After completion of installation, you need to add 'phpmyadmin' to the apache configuration.  

{% codeblock %}
sudo gedit /etc/apache2/apache2.conf
{% endcodeblock %}

Add the line to apache config file.  
{% codeblock %}
Include /etc/phpmyadmin/apache.conf
{% endcodeblock %}

Restart apache:  
{% codeblock %}
sudo service apache2 restart
{% endcodeblock %}

Congrats!!!  
You have installed the phpMyadmin.  
You can access it using url localhost/phpmyadmin in the browser.
