---
layout: post
title: "Sorting a CSV file using Python"
date: 2013-07-26 18:16
comments: true
categories: 
---
Today ,just got the the task to sort a CSV file. I tried it using Python, and completed the task.  
So here is my python script.  

``` ruby sort.py
			import sys, csv ,operator
			data = csv.reader(open('File.csv'),delimiter=',')
			sortedlist = sorted(data, key=operator.itemgetter(0))	# 0 specifies according to first column we want to sort
			#now write the sorte result into new CSV file
			with open("NewFile.csv", "wb") as f:
				fileWriter = csv.writer(f, delimiter=',')
				for row in sortedlist:
					fileWriter.writerow(row)
```
