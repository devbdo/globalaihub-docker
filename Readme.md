# 🐳 Docker + PHP 7.4 + MySQL + Nginx 

## Description

This is a complete stack for running gaih 5 into Docker containers using docker-compose tool.

It is composed by 3 containers:

- `nginx`, acting as the webserver.
- `php`, the PHP-FPM container with the 7.4 PHPversion.
- `db` which is the MySQL database container with a **MySQL 8.0** image.

## Installation


1. 😀 Run code

```bash
docker-compose up -d
```

2. The 3 containers are deployed: 

```
Creating gaih-docker_db_1    ... done
Creating gaih-docker_php_1   ... done
Creating gaih-docker_nginx_1 ... done
```

3. Use this value for the DATABASE_URL environment variable of gaih:

```bash
DATABASE_URL=mysql://gaih_user:gaih123*@db:3306/gaih_db?serverVersion=5.7
```

You could change the name, user and password of the database in the `env` file at the root of the project.

## Developer Süleyman Ekici

