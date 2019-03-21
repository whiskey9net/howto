### Cheat Sheet
```mysql
mysql> CREATE USER 'username'@'%'         IDENTIFIED BY 'passwrod';
mysql> CREATE USER 'username'@'localhost' IDENTIFIED BY 'passwrod';
 
mysql> ALTER USER 'username'@'localhost' IDENTIFIED BY 'passwrod';
  -- or
mysql> SET PASSWORD FOR 'username'@'localhost' ='passwrod'
 
mysql> CREATE DATABASE mydb;
 
mysql> GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
  -- The asterisks in this command refer to the database and table (respectively).
 
mysql> FLUSH PRIVILEGES;
 
-- Truncate table (drop and then re-create again (including any indexes and constraints)
mysql> TRUNCATE [TABLE] tbl_name
 
mysql> UPDATE mytable SET field1 = newvalue1, field2 = newvalue2 [WHERE Clause];
```
