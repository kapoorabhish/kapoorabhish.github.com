---
layout: post
title: "Setting Virtual Environment in Linux"
date: 2013-06-11 13:25
comments: true
categories: 
---
To set up a Virtual Environment, you first need to install <b>"virtualenvwrapper"</b>.  
{% codeblock %}
$ pip install virtualenvwrapper
{% endcodeblock %}
or
{% codeblock %}
$ pip easy_install virtualenvwrapper
{% endcodeblock %}

Setup:  
Create a directory to hold the virtual environments.  
{% codeblock %}
$ mkdir $HOME/.virtualenvs
{% endcodeblock %}


Now,make a environment variable which has the path of .virtualenvs  
{% codeblock %}
$ export WORKON_HOME=$HOME/.virtualenvs
{% endcodeblock %}  

Next run the shell script virtualenvwrapper.sh  
{% codeblock %}
$ source virtualenvwrapper.sh
{% endcodeblock %}  
Run: workon
{% codeblock %}
$ workon
{% endcodeblock %}

A list of environments, empty, is printed.  
Run: mkvirtualenv temp.  This includes A virtual environment "temp".
{% codeblock %}
$ mkvirtualenv temp. 
{% endcodeblock %}

Run: workon temp.
{% codeblock %}
$ workon temp
{% endcodeblock %}  

The virtual environment is activated.  

