# Test Case

## Web

1. Can you create a simple Web Page which handles Multi-users login using MERN or other framework you are familiar with?
2. Can you create a simple Calculator using JS, HTML & CSS? 
3. Create a simple ToDo App which includes ReactJs as front end and handle requests with NodeJs in [Repl.it](http://Repl.it) ?
4. [Make a counter app that will increase the number of counts as users click on the “Add” button using Functional].(https://www.geeksforgeeks.org/differences-between-functional-components-and-class-components-in-react/#:~:text=Make%20a%20counter%20app%20that%20will%20increase%20the%20number%20of%20counts%20as%20users%20click%20on%20the%20%E2%80%9CAdd%E2%80%9D%20button%20using%20Functional%20and%20Class%20components)

Functional Components: Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function.

Syntax:
```
const Car=()=> {
  return <h2>Hi, I am also a Car!</h2>;
}
```
Example:
```
import React ,{useState} from "react";
 
const FunctionalComponent=()=>{
    const[count , setCount]=useState(0);
 
    const increase=()=>{
        setCount(count+1);
    }
 
    return
        <div style={{margin:'50px'}}>
            <h1>Welcome to Geeks for Geeks </h1>
            <h3>Counter App using Functional Component : </h3>
          <h2>{count}</h2>
            <button onClick={increase}>Add</button>
        </div>
    )
} 
 
 
export default FunctionalComponent;
```



5.  With your knowledge in front-end Web Technologies, Create a Web page similar to the following attached image. You can use any of your favourite frameworks or use plane HTML, CSS and Vannila Js. You can upload the code on repl.it and share us the link.

Refer - https://github.com/mohamadadithya/frontend-mentor-challenges/tree/master/sunnyside-agency-landing-page-main

---

#Python:

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

