---
title: SQL Help
categories: Programming
version: all
top: true
---

## Role

#### Create user

###### PostgreSQL

```sql
CREATE USER uname WITH PASSWORD 'passwd';
```

###### MySQL

```sql
CREATE USER 'uname'@'host' identified by 'passwd';
```
#### Update user password


###### PostgreSQL
```sql
ALTER USER postgres WITH PASSWORD 'postgres';
```


###### MySQL

```sql
SET PASSWORD FOR 'uname'@'host' = PASSWORD("passwd");
```

#### Grant database privilege

###### PostgreSQL

```sql
GRANT ALL PRIVILEGES ON DATABASE dbname to uname;
```

###### MySQL

```sql
GRANT ALL ON dbname.* TO 'uname'@'host';

```



## Database

### Create datebase

###### PostgreSQL

```sql
CREATE DATABASE dbname OWNER uname;
```

###### MySQL

```sql
CREATE DATABASE dbname;
CREATE DATABASE dbname CHARACTER SET utf8;
```

