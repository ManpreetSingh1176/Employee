# Employee-API
Steps to be followed :
(Python dependency packages : Pymysql,Flask,pandas) - use pip install, brew install 
Unzip the attached code file

run the docker imagine for sample Mysql-employees

docker run -d \
  --name mysql-employees \
  -p 3306:3306 \
  -e MYSQL_ROOT_PASSWORD=college \
  -v $PWD/data:/var/lib/mysql \
  genschsa/mysql-employees
 
Execute the Flask.py
Open brower for http://127.0.0.1:5000/

Error Logging : Errorlog.txt (default:warning) 
Testing :

Landing page : "Welcome to Employee API!"

Operation 1 : http://127.0.0.1:5000/Operation1 
(Displays the list of top 10 emp_no)

Operation 2 : http://127.0.0.1:5000/Operation2
Prompts : Please enter a valid employee_no
<Enter the emp_no Authorized dictionay>
  
 Testcase 1 : http://127.0.0.1:5000/Operation2?emp_no=100003 (Displays the information and history of respective emp_no)
 Testcase 2 : http://127.0.0.1:5000/Operation2?emp_no= any ("Error: Emp_No not authenticated. Please Re-try.") 


