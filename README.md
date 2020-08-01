# php_mysql_dockerfiles
php_mysql_dockerfiles
Important Note:

Change your database username and password in db.php file.


Create Database Using the following Query:

CREATE DATABASE IF NOT EXISTS register;


and Create Tables either importing attached sql file (register.sql) or using the below 2 SQL queries:


CREATE TABLE IF NOT EXISTS register.`users` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `username` varchar(50) NOT NULL,
 `email` varchar(50) NOT NULL,
 `password` varchar(50) NOT NULL,
 `trn_date` datetime NOT NULL,
 PRIMARY KEY (`id`)
 );


CREATE TABLE IF NOT EXISTS register.`new_record` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `trn_date` datetime NOT NULL,
 `name` varchar(50) NOT NULL,
 `age`int(11) NOT NULL,
 `submittedby` varchar(50) NOT NULL,
 PRIMARY KEY (`id`)
 );

If It code will run without docker then DATABASE CREDENTIALS IS AVIALABLE IN .htaccess file because connectivity using Environment variables .Put src file and run PHP CRUD application. 
If PHP code shows some errors like "PHP - cannot modify header information - headers already sent by (output started at" then add ob_start(); at the start of all php files.
CREATD BY VINEET KUMAR
