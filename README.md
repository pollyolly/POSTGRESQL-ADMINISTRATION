## POSTGRESQL-ADMINISTRATION
### Remote Connection

[PostgreSQL Remote Connection](https://medium.com/@johnmark_76235/postgresql-remote-connection-with-pgadmin-on-a-virtual-private-server-ubuntu-f82bcc9e197c)

### Show all databases
```
postgres=#\list
```
### Create User
```sql
CREATE USER dianna WITH PASSWORD '12345678';
```
### Create Database
```sql
CREATE DATABASE dianna_db;
```
### Permission
```sql
-- Remove Access to Query
REVOKE ALL PRIVILEGES ON DATABASE dianna_db FROM other_username;
REVOKE ALL ON DATABASE dianna_db FROM PUBLIC;
-- Grant all privileges to user
GRANT ALL PRIVILEGES ON DATABASE "dianna_db" to dianna;
```
### Drop Database
```sql
DROP DATABASE dianna_db;
```
### Drop User
```sql
DROP USER dianna;
```
### Backup
[PostgreSQL Backup](https://medium.com/@johnmark_76235/postgresql-backup-5b2ca6956410)
