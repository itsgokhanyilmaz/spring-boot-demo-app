## SPRING-BOOT DEMO APP

This is a simple spring-boot demo application

### Prerequisites

- Java (11 or up)
- Docker
- Maven

### Getting the project

1.Create project folder:
```
$ mkdir <project-name>
$ cd <project-name>
```

2.Clone the project:
```
$ git clone https://github.com/itsgokhanyilmaz/spring-boot-demo-app.git
```

3.Create a docker container for PostgreSQL Database:
```
$ docker create --name postgres-demo -e POSTGRES_PASSWORD=Welcome -p 5432:5432 postgres:11.5-alpine
```
4.Start your container:
```
$ docker start postgres-demo
```
5.Connect to PostgreSQL console from docker and create a database:
```
$ docker exec -it postgres-demo psql -U postgres
postgres>> create database conference_app
```

6.Connect the database with DataGrip or pgAdmin or anything you want
```
Connection Info : 

JDBC URL :  jdbc:postgresql://localhost:5432/conference_app
Username :  postgres
Password :  Welcome 

```

7.Run sql scripts in the sql-scripts folder


## Authors
* **Gokhan YILMAZ** [profile](https://github.com/itsgokhanyilmaz)
