mydb = mysql.connector.connect(
  host="localhost",
  user="root",
  password="", 
)

print(mydb)
mycursor = mydb.cursor(buffered=True)
mycursor.execute("create database Game")

mycursor.execute("create table Teams(name varchar(30),id(5),country(30)")
mydb.commit()
