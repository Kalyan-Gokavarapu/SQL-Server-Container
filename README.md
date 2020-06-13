# SQL-Server-Container
Docker compose for spinning up a new SQL server container

Run the below command from the root path to spin a sql server container instance
``` yml
docker-compose up -d 
```

You can use a SQl Server Management Studio or any other tool to connect to the sql server instance

    Server: .
    Username: sa
    Password: sqlserver_password


You can connect to the server instance from PowerShell as well by using the below command
    docker exec -it sqlserver_container /opt/mssql-tools/bin/sqlcmd -S localhost -U sa -P sqlserver_password

Note: 
`sqlserver_container` is the container name and
`sqlserver_password` is the password for `sa` user
