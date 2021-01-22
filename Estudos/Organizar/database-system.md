# Notas Database Systems

## Livros

- [Database System Concepts](/BancoDeDados/Book_DatabaseSystemConcepts/notas_DatabaseSystemConcepts.md)

## Video aulas

- [15-445/645 Intro to Database Systems (Fall 2019)](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi)

## Estudar mais

- Relation Algebra

# SQL
#Estudos/DataScience/BancoDeDados
## Roadmap
	- [ ] [[Livro: Database System Concepts - Silberschatz, Korth, Sudarshan]]
	- [ ] [15-445/645 Intro to Database Systems (Fall 2019) - YouTube](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi)
	- [ ] [15-721 Advanced Database Systems (Spring 2019) - YouTube](https://www.youtube.com/playlist?list=PLSE8ODhjZXja7K1hjZ01UTVDnGQdx5v5U)
	- [ ] [Engenharia de Computação - Bancos de Dados](https://www.youtube.com/playlist?list=PLxI8Can9yAHeHQr2McJ01e-ANyh3K0Lfq)
	
## Autores de Referência
	- C. J. Date
	- Abraham Silberschatz
	- Ramez Elmasri

## Bibliografia
	- [ ] An Introduction to Database Systems - C. J. Date

## Tools
### Diagrams Design
	- [PonyORM - Python ORM with beautiful query syntax](https://ponyorm.org/)
	- [relational algebra calculator](https://dbis-uibk.github.io/relax/calc.htm)

### Databases Systems
	- [Db2 Database - IBM](https://www.ibm.com/products/db2-database)
	- Microsoft SQL Server
	- PostgreSQL
	- SQLite

	- [dbdiagram.io - Database Relationship Diagrams Design Tool](https://dbdiagram.io)
	- [Home - QuickDBD](https://www.quickdatabasediagrams.com/)
	- [SQL Database Modeler - SQL Database Modeler, Entity Relationship Diagram](https://sqldbm.com/Home/)
	- 


## Pesquisar mais sobre
- [ ] SQL Server 
- [ ] Mongo DB
- [ ] Regis
- [ ] Cassandra
- [ ] Neo 4J
- [ ] Álgebra Relacional 
- [ ] Cálculo Relacional
	

[Learn SQL | Vertabelo Academy](https://academy.vertabelo.com/#courses_list_section)

*## LIVROS*
 - [ ] Head First SQL - 


# Notas Database Systems

## Livros

- [] [Database System Concepts](/BancoDeDados/Book_DatabaseSystemConcepts/notas_DatabaseSystemConcepts.md)

## Video aulas

- [] [15-445/645 Intro to Database Systems (Fall 2019)](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi)

## Estudar mais

- Relation Algebra

# SQL
#Estudos/DataScience/BancoDeDados
## Roadmap

	- [ ] [15-721 Advanced Database Systems (Spring 2019) - YouTube](https://www.youtube.com/playlist?list=PLSE8ODhjZXja7K1hjZ01UTVDnGQdx5v5U)
	- [ ] [Engenharia de Computação - Bancos de Dados](https://www.youtube.com/playlist?list=PLxI8Can9yAHeHQr2McJ01e-ANyh3K0Lfq)
	
## Autores de Referência
	- C. J. Date
	- Abraham Silberschatz
	- Ramez Elmasri

## Bibliografia
	- [ ] An Introduction to Database Systems - C. J. Date

## Tools
### Diagrams Design
	- [PonyORM - Python ORM with beautiful query syntax](https://ponyorm.org/)
	- [relational algebra calculator](https://dbis-uibk.github.io/relax/calc.htm)

### Databases Systems
	- [Db2 Database - IBM](https://www.ibm.com/products/db2-database)
	- Microsoft SQL Server
	- PostgreSQL
	- SQLite

	- [dbdiagram.io - Database Relationship Diagrams Design Tool](https://dbdiagram.io)
	- [Home - QuickDBD](https://www.quickdatabasediagrams.com/)
	- [SQL Database Modeler - SQL Database Modeler, Entity Relationship Diagram](https://sqldbm.com/Home/)
	- 


## Pesquisar mais sobre
- [ ] SQL Server 
- [ ] Mongo DB
- [ ] Regis
- [ ] Cassandra
- [ ] Neo 4J
- [ ] Álgebra Relacional 
- [ ] Cálculo Relacional
	

[Learn SQL | Vertabelo Academy](https://academy.vertabelo.com/#courses_list_section)

*## LIVROS*
 - [ ] Head First SQL - 



dbKoda.com

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

dbKoda.com
