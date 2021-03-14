# NOTAS DE ESTUDO: DATABASE SYSTEM

## Docker

> Criar um container rodando o SQL Server

```bash
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=yourStrong(!)Password' -e 'MSSQL_PID=Express' -p 1433:1433 -d mcr.microsoft.com/mssql/server
```
> Acessar o container e a cli do SQL Server
```bash
docker exec -it <container_id|container_name> /opt/mssql-tools/bin/sqlcmd -S localhost -U sa
```
