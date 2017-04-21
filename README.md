# docker-php-mysql

Create a simply cakePHP3 project on Docker

## Please prepare in advance

> install docker ->
 [https://www.docker.com/](https://www.docker.com/)

## clone

```git clone  https://github.com/shirabelass1001/docker-php-mysql.git```

## run

```$ docker-compose up -d```

## Create cakePHP

```$ docker-compose run --rm php composer create-project --prefer-dist -n cakephp/app app```

## edit config

### 1. edit working directry

> .env 15 line

```WORK_DIRPATH=/yourDirectoryPath/docker-php-mysql```

### 2. change default setting (for connect to the database)

```cd webapps/app/config/app.php```

> app.php 225 line

before

```'host' => 'localhost',```

after

```'host' => 'my_mysql',```

## check

[http://localhost:8765/app/](http://localhost:8765/app/)
