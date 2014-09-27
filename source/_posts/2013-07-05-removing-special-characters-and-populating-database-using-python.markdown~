---
layout: post
title: "Removing Special Characters &amp; Populating Database using Python"
date: 2013-07-05 21:59
comments: true
categories: Python MySQL Database Excel
---
<table>
<th>State Name</th>
<th>Village Name</th>
<th>Habitation Name</th>
<tr>
<td>ANDHRA PRADESH    &nbsp;</td>
<td>J.K.GUMADA(001 )    &nbsp;</td>
<td>J.K.GUMADA (0101302001010100)</td>
</tr>
<tr>
<td>ANDHRA PRADESH    &nbsp;</td>
<td>V.V.R.PETA(002 )    &nbsp;</td>
<td>V.V.R.PETA(0101302002010100)</td>
</tr>
</table>  


If a table as shown above is there which contains some text, numbers and some special characters and we need to populate our database after removing all the numbers and special characters.  
Here I am posting a Python script to complete the task.  

``` ruby populatedata.py
	import xlrd
	import MySQLdb
	import re

	# Open the workbook and define the worksheet
	book= xlrd.open_workbook("testdata1.xls")
	sheet = book.sheet_by_name("testdata1")

	# Establish a MySQL connection
	database = MySQLdb.connect (host="localhost", user = "username", passwd = "password", db = "database_name")

	# Get the cursor, which is used to traverse the database, line by line
	cursor = database.cursor()

	# Create the INSERT INTO sql query


	query = """INSERT INTO testdata  VALUES (%s,%s,%s)"""
	
	
	# Create a For loop to iterate through each row in the XLS file, starting at row 2 to skip the headers
	for r in range(1, sheet.nrows):
		#first remove the numbers
		state=re.sub("\d+","",sheet.cell(r,0).value)
		#then remove the last two remaining brackets
		state=state[:-2]
		village=re.sub("\d+","",sheet.cell(r,4).value)
		village=village[:-2]
		habitation=re.sub("\d+","",sheet.cell(r,5).value)
		habitation=habitation[:-2]
		
	# Assign values from each row
	values =(state,district,block,panchayat,village,habitation)
	# Execute sql Query
	try:
		
		cursor.execute(query,values)
	except:
		pass



	# Close the cursor
	cursor.close()

	# Commit the transaction
	database.commit()

	# Close the database connection
	database.close()

```

Hope this script will help you!!!

