---
layout: post
title: "Accesing csv file using Shell Script"
date: 2013-06-14 08:19
comments: true
categories: 
---
Given a text file in which there are links of file to be dowloaded (one link per line), here I am posting a shell script to achieve the task.


			myfilename=/home/abhishek/Desktop/ideas.txt		#here path to txt file has been stored in $myfilename
			while read line
			do
		
				curl --remote-name $line

			done		<$myfilename


The above shell script reads the ideas.txt file line by line and download all the files in the current directory.
