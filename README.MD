## Create Docker with Apache/PHP and Mysql for Laravel App

* Edit **.env** file with your settings

* Run 
```
docker-compose up -d
```

* It will create 2 containers (Apache Server and Mysql Server)

* **/www** folder will be created

* Put your laravel application files in **/www** folder

* Edit Laravel .env file, install depedencies, migrations etc

* Mysql data files will be in **/docker/mysql/data** folder

You can create your apache image instead of **apps4net/laravel-apache** with the command:

```
docker build -t apache docker/apache
```

Thne use this at **docker-compose.yml** file

``` 
image: apache
```