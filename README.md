## Prerequisites
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later

## Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
## Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

## Docker_setup
1) create dockerfiles for app , web , db 
2) dont forget to move .war file in app folder , .sql in db folder , nginx.conf in web folder (as mwntioned in dockerfile)
3) create docker images with name as app , db , web from above dockerfiles and pull rabbitmq and memcached
4) create docker-compose file 
5) In docker-compose contaienrs name,port numbers should be same as you mentioned in /root/vprofile-project/src/main/resources/application.properties


Then look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql


