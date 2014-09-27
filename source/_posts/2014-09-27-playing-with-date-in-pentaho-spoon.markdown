---
layout: post
title: "Playing with Date in Pentaho Spoon"
date: 2014-09-27 19:10
comments: true
categories: Pentaho Date Spoon Kettle
---
I got the date in which there was a date field in form __dd/mm/yy__ and I needed to convert into the format of __dd/mm/yyyy__.  
Oops!!! How to specify the year 2000 in the date, coz in the date format meta data i can change format to dd/mm/yyyy but can't specify the year number.  
Then, something hit into my mind and I specified the format as __dd/mm/20yy__ and Bingo!!!  

The sample transformation can be downloaded <a href="https://github.com/kapoorabhish/kapoorabhish.github.com/blob/source/source/kettle_transformation/playing_with_date.ktr.zip?raw=true">__here__</a>.


