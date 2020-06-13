# SQL-Server-Container
Docker compose for spinning up a new SQL server container

#### Run the below command to the root path to spin a sql server ina container
``` yml
docker-compose up -d 
```

#### You can use a SQl Server Management Studio or any other tool to connect to the sql server

    Server: .
    Username: sa
    Password: sqlserver_password


#### Use the below command to connect to sql server from PS
    docker exec -it sqlserver_container /opt/mssql-tools/bin/sqlcmd -S localhost -U sa -P sqlserver_password

####  Note: 
######  sqlserver_container is the container name
###### sqlserver_password is the password for sa user
