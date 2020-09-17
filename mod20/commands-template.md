# Template for commands and secrets

This template can be prepared as described here, and used during the presentations.

Save a copy of this file and replace the expressions in `[]` below according to the notes.

> **IMPORTANT**: Do not commit this file in any Github public repo after you edit it. Connection strings and other secrets should never be committed to a public repository.

## Preparation before the demos:

### Credentials

```
Username: demouser
Password: Azuredemo2020
```

### Mongo VM connection string

```
mongodb://168.63.232.13:27017
```

### SQL Server 2012 connection string

```
Server=tcp:168.63.250.23,1433;Initial Catalog=tailwindsql;Persist Security Info=False;User ID=demouser;Password=Azuredemo2020;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=True;Connection Timeout=30;
```

### Mongo DB VM

```
ssh demouser@168.63.232.13
password: Azuredemo2020
```

### Remote desktop SQL Server VM

```
IP address: 168.63.250.23
Username: demouser
Password: Azuredemo2020
```

### Tailwindtraders website

```
Username: cxo@microsoft.com
Password: 1234
```

### Azure SQL DB

```
Username: demouser
Password: Azuredemo2020
```

## Demo 1: MongoDB to CosmosDB migration

### Mongo DB VM

```
ssh demouser@168.63.232.13
password: Azuredemo2020
```

### Tailwindtraders website

```
Username: cxo@microsoft.com
Password: 1234
```

### Source connection string

```
mongodb://168.63.232.13:27017
```

### Target connection string

```
mongodb://mod20judecosmos:GQOCRDZakFqxUEFVIre69tHfhBYtkdAWgG7NW73y5w38dtbwKkY8NHNTrsm6E3VpBi4LnxlHWUDXWpmHC0YXOg==@mod20judecosmos.documents.azure.com:10255/?ssl=true&replicaSet=globaldb
```

### BAK target connection string

```
mongodb://mod20judecosmos-bak:tobhO05fMqtQylYGBKQnoeNzpEvnOybpCPTw33KKKJJOk0ibQFN2dRQG1lXphNZODgbQnuNEk4Fb7A4zPsA7uA==@mod20judecosmos-bak.documents.azure.com:10255/?ssl=true&replicaSet=globaldb
```

### Cart item:

```
{
	"_id" : "5d665a5689c79d19d44b4799",
	"productId" : 99,
	"email" : "cxo@microsoft.com",
	"imageUrl" : "https://github.com/ashleymcnamara/Developer-Advocate-Bit/blob/master/BitDevAdvocate.png?raw=true",
	"name" : "Cloud Advocate Mascot",
	"price" : "999",
	"qty" : 3,
	"id" : "f2729f14-090d-4b40-8e45-e5dcdb58c0a2"
}
```

## Demo 2: SQL to Azure SQL DB migration

### Source SQL

```
IP: 168.63.250.23
Username: demouser
Password: Azuredemo2020
```

### Target SQL credentials (for Database migration service)

```
Host name: mod20judesqlsvr.database.windows.net
Username: demouser
Password: Azuredemo2020
```

### Target SQL Connection string

```
Server=tcp:mod20judesqlsvr.database.windows.net,1433;Initial Catalog=mod20judesqldb;Persist Security Info=False;User ID=demouser;Password=Azuredemo2020;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;
```

### Target BAK SQL Connection string

```
Server=tcp:mod20judesqlsvr.database.windows.net,1433;Initial Catalog=mod20judesqldb-bak;Persist Security Info=False;User ID=demouser;Password=Azuredemo2020;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;
```
