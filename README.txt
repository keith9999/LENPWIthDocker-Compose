Note:
Please prepare follow item install into you Linux:
docker,
docker-mechine,
docker-compose,
virtualbox,



Run command:

step 1:
docker-compose up -d

step 2:
then it will create 4 containers:
you can use command to check:

docker ps

the result will list follow items:
1. dockerlemp_nginx_1
2. dockerlemp_phpmyadmin_1
3. dockerlemp_phpfpm_1
4. dockerlemp_mysql_1

step 3:
go to web browser,
type 

localhost:80

then will open PHP page

step 4:
still go to web browser
type
localhost:8183

then you will see the phpMyAdmin login page

step 5:
at the terminal

type 

docker ps

then type

docker-compose exec mysql sh

then type

mysql -u root -p

then type password

admin

then type

show databases;

then you will see the database table

then type

exit

then type exit

step 6: stop docker-compose

in the terminal

type command

docker-compose stop

then type command

docker ps

then type command

docker-compse stop

then if you want to remove the containers then type command

docker-compose rm --all
