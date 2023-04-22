# Docker Compose Develop Environment

## Overview
With Docker Compose, you can run multiple Dockers in a local environment.  

By assigning each Docker the role of application, DB, and AWS, you can develop code for cloud development in a local environment at high speed.  

In this repository, we have a LocalStack that can emulate AWS and a Docker for PostgreSQL.  

Please add a Docker for your favorite application to build a local environment for cloud development.  


## Command Memo
### Docker Compose Command Memo
$ sudo docker-compose build  
$ docker-compose up -d  
$ docker-compose stop  
$ docker-compose down  

### LocalStack(AWS) Command Memo
$ aws s3 mb s3://local-backet --endpoint-url=http://localhost:4566  
$ aws s3 cp TEST.txt s3://local-backet/test/ --endpoint-url=http://localhost:4566  
$ aws s3 ls s3://local-backet/test/ --endpoint-url=http://localhost:4566  
   
### DB Command Memo
$ docker-compose exec db psql -U postgres  
$ sudo chmod 755 ./postgres-data  
