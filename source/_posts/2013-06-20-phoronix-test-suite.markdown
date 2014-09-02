---
layout: post
title: "Phoronix Test Suite"
date: 2013-06-20 13:02
comments: true
categories: 
---
I got a task to test a server which we made and named it <b>Ant</b>.It has <b>Centos 6</b> installed on it.  
As suggested I made use of <b>Phoronix Test Suite</b>.  
So here I am posting how to install it on Centos.  


<h3>Phoronix Test Suite- An Automated, Open-Source Testing Framework</h3>
The Phoronix Test Suite is the most comprehensive testing and benchmarking platform available for the Linux operating system. This software is designed to effectively carry out both qualitative and quantitative benchmarks in a clean, reproducible, and easy-to-use manner. The Phoronix Test Suite consists of a lightweight processing core (pts-core) with each benchmark consisting of an XML-based profile with related resource scripts. The process from the benchmark installation, to the actual benchmarking, to the parsing of important hardware and software components is heavily automated and completely repeatable, asking users only for confirmation of actions.  

<a href="http://pkgs.org/centos-6-rhel-6/epel-i386/phoronix-test-suite-3.8.0-1.el6.noarch.rpm/download/" targe=_blank>Download phoronix-test-suite</a>
``` ruby Install Howto


    Download the latest epel-release rpm from

    http://dl.fedoraproject.org/pub/epel/6/i386/

    Install epel-release rpm:

    # rpm -Uvh epel-release*rpm

    Install phoronix-test-suite rpm package:

    # yum install phoronix-test-suite
```


<h6>from-pkgs.org</h6>


