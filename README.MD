# Portfolio_Global

The project called `Portfolio`:

At this point, the project layout look like the following:

```text
my-app/
├─ _doc/
│  └─ ...
├─ docker/
│  └─ apache
│  └─ config
│  └─ mysql
│  └─ nginx
│  └─ node
│  └─ php
├─ Front    -> Angular/
│  └─ ...
├─ Back     -> SYMFONY 4/
│  └─ ...
└─ docker-compose.yml
```

## Docker containers:

		DataBase:
		 1. MySQL
		 2. PhpMyAdmin
		
		Server Code:
		 1. PHP
		 2. Apache
	 
		 Front End Code:
		 1. NGINX


Usage
-----
Run development environment
```bash
$ docker-compose up
```
or run in background
```bash
$ docker-compose up -d
```
To down environment
```bash
$ docker-compose down
```
Useful
------
Show all container
```bash
$ docker-compose ps
```
Connect to container
```bash
$ docker exec -it {container_name} bash
```
Fix minor problem with docker images
```bash
$ docker-compose up --force-recreate
```

Hacks
-----
For correct work with angular app you must fix `package.json`
```
"scripts": {
    "ng": "ng",
    "start": "ng serve --host 0.0.0.0",
    ....
```

Access to Url's
------------------
Symfony: http://localhost:82

Angular: http://localhost:4200

Phpmyadmin: http://localhost:8080

ApiDoc: http://localhost:82/swagger/index.html

## Versioning
[<img src='https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/Octicons-mark-github.svg/1200px-Octicons-mark-github.svg.png' width='30' />
](https://github.com/) - **Github**, Web-based version-control and collaboration platform for software developers.

## Authors

* [**Franck GARCON**](https://github.com/Franckeddy)
