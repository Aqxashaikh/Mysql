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
import mysql.connector

mydb = mysql.connector.connect(
  host="localhost",
  user="myusername",
  password="mypassword",
  database="mydatabase"
)

mycursor = mydb.cursor()

mycursor.execute("CREATE TABLE customers (name VARCHAR(255), address VARCHAR(255))")
cursor = conn.cursor()

Show databases
cursor.execute("SHOW DATABASES;")
for db in cursor.fetchall():
    print(db)

cursor.close()
conn.close()
