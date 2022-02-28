Python Challenges:

1. Write a Python program to list only directories, files and all directories, files in a specified path
(Refer: https://www.w3resource.com/python-exercises/os/index.php)

A) Python Code :
  ```
import os
path = 'g:\\testpath\\'
print("Only directories:")
print([ name for name in os.listdir(path) if os.path.isdir(os.path.join(path, name)) ])
print("\nOnly files:")
print([ name for name in os.listdir(path) if not os.path.isdir(os.path.join(path, name)) ])
print("\nAll directories and files :")
print([ name for name in os.listdir(path)])
  ```
sample output: 
   ```
Only directories:
['dev', 'boot', 'proc', 'sys', 'sbin', 'lib32', 'srv', 'etc', 'tmp', 'libx32', 'mnt', 'bin', 'usr', 'opt', 'root', 'run', 'media', 'var', 'home', 'lib64', 'lib', 'trinket', 'bd_build']

Only files:
['.dockerenv', 'get-pip.py']

All directories and files :
['dev', 'boot', 'proc', 'sys', 'sbin', 'lib32', 'srv', 'etc', 'tmp', 'libx32', 'mnt', 'bin', 'usr', 'opt', 'root', 'run', 'media', 'var', 'home', 'lib64', 'lib', '.dockerenv', 'trinket', 'get-pip.py', 'bd_build']
  ```




2. Write a Python program to read a given CSV file as a dictionary
(refer: https://www.w3resource.com/python-exercises/csv/index.php)

A) Sample Solution:

  Python Code :
  ```
import csv
with open('departments.csv', newline='') as csvfile:
 data = csv.DictReader(csvfile)
 print("ID Department Name")
 print("---------------------------------")
 for row in data:
   print(row['department_id'], row['department_name'])
  ```
  
  CSV file contents:
  ```
department_id,department_name,manager_id,location_id
10,Administration,200,1700
20,Marketing,201,1800
30,Purchasing,114,1700
40,Human Resources,203,2400
50,Shipping,121,1500
60,IT,103,1400
70,Public Relations,204,2700
80,Sales,145,2500
90,Executive,100,1700
100,Finance,108,1700
110,Accounting,205,1700
120,Treasury,,1700
130,Corporate Tax,,1700
140,Control And Credit,,1700
150,Shareholder Services,,1700
160,Benefits,,1700
170,Manufacturing,,1700
180,Construction,,1700
190,Contracting,,1700
200,Operations,,1700
210,IT Support,,1700
220,NOC,,1700
230,IT Helpdesk,,1700
240,Government Sales,,1700
250,Retail Sales,,1700
260,Recruiting,,1700
270,Payroll,,1700
```
  Sample Output:
```
ID Department Name
---------------------------------
10 Administration
20 Marketing
30 Purchasing
40 Human Resources
50 Shipping
60 IT
70 Public Relations
80 Sales
90 Executive
100 Finance
110 Accounting
120 Treasury
130 Corporate Tax
140 Control And Credit
150 Shareholder Services
160 Benefits
170 Manufacturing
180 Construction
190 Contracting
200 Operations
210 IT Support
220 NOC
230 IT Helpdesk
240 Government Sales
250 Retail Sales
260 Recruiting
270 Payroll
```


3.Python program to find all non repeating characters in the string

A. https://quescol.com/interview-preparation/print-maximum-character-string-python

