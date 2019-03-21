### Cheat Sheet
```mysql
-- USERS ------------------------------------------------------------------------------

CREATE USER 'username'@'%'         IDENTIFIED BY 'passwrod';
CREATE USER 'username'@'localhost' IDENTIFIED BY 'passwrod';
 
ALTER USER 'username'@'localhost' IDENTIFIED BY 'passwrod';
  -- or
SET PASSWORD FOR 'username'@'localhost' ='passwrod'

SELECT User, Host FROM mysql.user;

CREATE DATABASE mydb;
 
GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
  -- The asterisks in this command refer to the database and table (respectively).
 
FLUSH PRIVILEGES;

-- DATABASES AND TABLES --------------------------------------------------------------

-- Truncate table (drop and then re-create again (including any indexes and constraints)
TRUNCATE [TABLE] tbl_name
 
UPDATE mytable SET field1 = newvalue1, field2 = newvalue2 [WHERE Clause];
```
