---
layout: post
title: "Reliance Net Connect on Ubuntu-12.04"
date: 2014-07-07 21:29
comments: true
categories: 
---
After surfing so many posts on Internet about installing and running Reliance Net Connect on Ubuntu, finally I was successful.
I have HUAWEI (model no. HUAWEI EC1262).

So, here I am going to explain step by step configuration.

First, install Wvdial.
(You may temporarily use wifi connection for all these, so that you need not to download these on separate machine or if you like you can.)
{% codeblock %}
$ sudo apt-get install wvdial
{% endcodeblock %}

Also install other packages required.
{% codeblock %}
$ sudo apt-get install libuniconf4.6 libwvstreams4.6-base libwvstreams4.6-extras wvdial
{% endcodeblock %}

Type in the following command to create wvdial.conf
{% codeblock %}
$ sudo wvdialconf /etc/wvdial.conf
{% endcodeblock %}
Next, open up the wvdial.conf file.
{% codeblock %}
$ sudo gedit /etc/wvdail.conf
{% endcodeblock %}

Here, are the contents of file. Some of the lines may differ, if line missing from mentioned below add them.
```ruby /etc/wvdail.conf
			[Dialer Defaults]
			Init1 = ATZ
			Init2 = ATQ0 V1 E1 S0=0 &C1 &D2 +FCLASS=0
			Modem Type = Analog Modem
			ISDN = 0
			New PPPD = yes
			Baud = 9600
			Modem = /dev/ttyUSB0
			Username = "Add reliance netconnect phone number here with out quotes"
			Password = "Add reliance netconnect phone number here with out quotes"
			Phone = #777
			Stupid Mode = 1
```
At last, open up the terminal give the following command
{% codeblock %}
$ sudo wvdial
{% endcodeblock %}

I hope your connection will be successful, and the output will be like this.
{% img center "{{ root_url }} /images/terminal.png" %}

Note: Keep the terminal window open till you want to use internet. When you want to close connection, press <b>ctrl+c</b>.
