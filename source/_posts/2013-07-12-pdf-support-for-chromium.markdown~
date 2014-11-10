---
layout: post
title: "pdf support for Chromium"
date: 2013-07-12 22:12
comments: true
categories: Chromium PDF Acroread
---
I didn't have pdf format support in my Chromium Browser. So I tried the following commands for it.   
{% codeblock %}
$ sudo apt-get install acroread
$ sudo apt-get install mozplugger
{% endcodeblock %}  


Next, open thwe file /etc/mozpluggerrc as a superuser.
{% codeblock %}
$ sudo gedit /etc/mozpluggerrc
{% endcodeblock %}  

Change the line which reads  
{% codeblock %}
define(ACROREAD, [repeat swallow(acroread) fill : acroread -openInNewWindow /a "$fragment" "$file"])
{% endcodeblock %}  
 
 To
 
{% codeblock %}
 define(ACROREAD, [repeat needs_xembed swallow(acroread) fill : acroread -openInNewWindow /a "$fragment" "$file"])
{% endcodeblock %} 

