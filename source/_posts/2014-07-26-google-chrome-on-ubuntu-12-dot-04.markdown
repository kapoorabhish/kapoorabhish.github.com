---
layout: post
title: "Google Chrome on Ubuntu-12.04"
date: 2014-07-26 19:56
comments: true
categories: 
---
On linux(Ubuntu) you can install Chromium browser using apt-get, but to install __Chrome__ you need to run some commands to make it install using apt-get.<br>
First, get a repository key and add it to your system.
{% codeblock %}
$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - 
{% endcodeblock %}

And, add the google repository to your source list.
{% codeblock %}
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
{% endcodeblock %}

Next, update your sources.
{% codeblock %}
sudo apt-get update
{% endcodeblock %}

Finally, install __google-chrome__.
{% codeblock %}
sudo apt-get install google-chrome-stable
{% endcodeblock %}

Hope, this will be helpful for you.
