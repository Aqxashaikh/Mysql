# Mysql
https://www.mysql.com/downloads/.
Download and install "MySQL Connector":

pip install mysql-connector-python

C:\Users\Your Name\AppData\Local\Programs\Python\Python36-32\Scripts>python -m pip install mysql-connector-python
import mysql.connector

mydb = mysql.connector.connect(
  host="localhost",
  user="yourusername",
  password="yourpassword"
)

print(mydb)
