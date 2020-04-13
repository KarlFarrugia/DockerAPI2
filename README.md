# DockerAPI2
A .Net Core api connected to an sql instance both hosted on docker following https://www.youtube.com/watch?v=4V7CwC_4oss

docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Pa55w0rd2019' -e 'MSSQL_PID=Express' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2017-latest-ubuntu

dotnet run

docker build -t kfarrugia/colourapi .

docker run -p 8080:80 kfarrugia/colourapi

docker-compose up
