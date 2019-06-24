1.Login
#mysql -u root -p

2.Create User
You Have always the Permission to create a new user in databases

CREATE USER 'someuser'@'localhost' IDENTIFIED BY 'somepassword';

#Taking NOTE ON THE CONVENTION 'CAPS FOR THE QUERIES'(Increases readability)

3.Viewing all the Users

#SELECT User, Host FROM mysql.user;
