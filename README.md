# Docker Compose Develop Environment

## Overview
Todo

## Command Memo
### LocalStack(AWS) Command Memo
$ aws s3 mb s3://local-backet --endpoint-url=http://localhost:4566  
$ aws s3 cp TEST.txt s3://local-backet/test/ --endpoint-url=http://localhost:4566  
$ aws s3 ls s3://local-backet/test/ --endpoint-url=http://localhost:4566  
   
### DB Command Memo
$ docker-compose exec db psql -U postgres  
$ sudo chmod 755 ./postgres-data  
