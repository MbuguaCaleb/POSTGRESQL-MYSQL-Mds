# MYSQL

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

MySQL COMMANDS

- EASY TO REMEMBER

```sh
$ mysql -u root -p

```

2.Create User

```sh
$ CREATE USER 'someuser'@'localhost' IDENTIFIED BY 'somepassword';

```

3.Viewing all the Users

```sh
$ SELECT User, Host FROM mysql.user;

```

4.Grant All Priveleges On All Databases

User access Rights /Priviledges

```sh
GRANT ALL PRIVILEGES ON _ . _ TO 'someuser'@'localhost';
```

```sh
FLUSH PRIVILEGES;
```

-Flush Priviledges clears the grants table.

5.SHOW GRANTS(CHECK USER PRIVILEDGES)

```sh
SHOW GRANTS FOR 'someuser'@'localhost';
```

6.Remove Grants

```sh
REVOKE ALL PRIVILEGES, GRANT OPTION FROM 'someuser'@'localhost';
```

7.Delete User

```sh

DROP USER 'someuser'@'localhost';

```

8.Exit

```sh
exit;
```

9.SHOW DATABASES

```sh
SHOW DATABASES
```

10.CREATE DATABASES

```sh
CREATE DATABASE acme;

```

11.Delete Database

```sh
DROP DATABASE acme;
```

12.SELECT DATABASE

```sh
USE acme;
```

13.CREATE TABLE

```sh
CREATE TABLE users(
id INT AUTO_INCREMENT,
first_name VARCHAR(100),
last_name VARCHAR(100),
email VARCHAR(50),
password VARCHAR(20),
location VARCHAR(100),
dept VARCHAR(100),
is_admin TINYINT(1),
register_date DATETIME,
PRIMARY KEY(id)
);
```

14.Delete / Drop Table

```sh
DROP TABLE tablename;
```

15.Show Tables

```sh
SHOW TABLES;
```

16.Insert Row / Record

```sh
INSERT INTO users (first_name, last_name, email, password, location, dept, is_admin, register_date) values ('Caleb', 'Mbugua', 'mbuguacaleb30@gmail.com', '123456','Naivasha', 'PROGRAMMER', 1, now());
```

17.Insert Multiple Rows

```sh
INSERT INTO users (first_name, last_name, email, password, location, dept, is_admin, register_date) values ('Fred', 'Smith', 'fred@gmail.com', '123456', 'New York', 'design', 0, now()), ('Sara', 'Watson', 'sara@gmail.com', '123456', 'New York', 'design', 0, now()),('Will', 'Jackson', 'will@yahoo.com', '123456', 'Rhode Island', 'development', 1, now()),('Paula', 'Johnson', 'paula@yahoo.com', '123456', 'Massachusetts', 'sales', 0, now()),('Tom', 'Spears', 'tom@yahoo.com', '123456', 'Massachusetts', 'sales', 0, now());
```
