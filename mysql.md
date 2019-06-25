# MYSQL

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

Dillinger is a cloud-enabled, mobile-ready, offline-storage, AngularJS powered HTML5 Markdown editor.

- Type some Markdown on the left
- See HTML in the right
- Magic

###mysql -u root -p

2.Create User
You Have always the Permission to create a new user in databases

CREATE USER 'someuser'@'localhost' IDENTIFIED BY 'somepassword';

###Taking NOTE ON THE CONVENTION 'CAPS FOR THE QUERIES'(Increases readability)

3.Viewing all the Users

###SELECT User, Host FROM mysql.user;

4.Grant All Priveleges On All Databases

User access Rights /Priviledges

###GRANT ALL PRIVILEGES ON _ . _ TO 'someuser'@'localhost';

###FLUSH PRIVILEGES;

Flush Priviledges clears the grants table.

5.SHOW GRANTS(CHECK USER PRIVILEDGES)

#SHOW GRANTS FOR 'someuser'@'localhost';

6.Remove Grants

REVOKE ALL PRIVILEGES, GRANT OPTION FROM 'someuser'@'localhost';

7.Delete User

#DROP USER 'someuser'@'localhost';

8.Exit

#exit;

9.SHOW DATABASES

#SHOW DATABASES

10.CREATE DATABASES

#CREATE DATABASE acme;

11.Delete Database
#DROP DATABASE acme;

12.SELECT DATABASE

#USE acme;

13.CREATE TABLE

#CREATE TABLE users(
#id INT AUTO_INCREMENT,
#first_name VARCHAR(100),
#last_name VARCHAR(100),
#email VARCHAR(50),
#password VARCHAR(20),
#location VARCHAR(100),
#dept VARCHAR(100),
#is_admin TINYINT(1),
#register_date DATETIME,
#PRIMARY KEY(id)
#);

14.Delete / Drop Table

#DROP TABLE tablename;

15.Show Tables

#SHOW TABLES;

16.Insert Row / Record

#INSERT INTO users (first_name, last_name, email, password, location, dept, is_admin, register_date) #values ('Caleb', 'Mbugua', 'mbuguacaleb30@gmail.com', '123456','Naivasha', 'PROGRAMMER', 1, now());

17.Insert Multiple Rows

#INSERT INTO users (first_name, last_name, email, password, location, dept, is_admin, register_date) values ('Fred', 'Smith', 'fred@gmail.com', '123456', 'New York', 'design', 0, now()), ('Sara', 'Watson', 'sara@gmail.com', '123456', 'New York', 'design', 0, now()),('Will', 'Jackson', 'will@yahoo.com', '123456', 'Rhode Island', 'development', 1, now()),('Paula', 'Johnson', 'paula@yahoo.com', '123456', 'Massachusetts', 'sales', 0, now()),('Tom', 'Spears', 'tom@yahoo.com', '123456', 'Massachusetts', 'sales', 0, now());
