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

DATABASE CREDENTIALS IS AVIALABLE IN .htaccess file because connectivity using Environment variables.Put src file and run PHP CRUD application 
CREATD BY VINEET KUMAR
