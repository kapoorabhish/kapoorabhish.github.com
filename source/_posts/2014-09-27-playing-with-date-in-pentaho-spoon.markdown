---
layout: post
title: "Playing with Date in Pentaho Spoon"
date: 2014-09-27 19:10
comments: true
categories: Pentaho Date Spoon Kettle
---
I got the date in which there was a date field in form dd/mm/yy and I needed to convert into the format of dd/mm/yyyy.<br>
Oops!!! How to specify the year 2000 in the date, coz in the date format meta data i can change format to dd/mm/yyyy but can't specify the year number.<br>
Then, something hit into my mind and I specified the format as dd/mm/20yy and Bingo!!!<br>

The sample transformation can be downloaded here.
