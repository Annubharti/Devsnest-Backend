# SQL
DB == Drives
Schemas == Folders

Create a Schema: create schema {schemaName};

Create a table in a Schema: create table {schemaName}.{tableName};

List all tables in a Schema: \d {schemaName}.*;

View a specific table: \d {schemaName}.{tableName};

Drop Schema: If(empty Schema): drop schema {schemaName};

else: drop schema {schemaName} cascade;


Tables in schema are objects.
A schema is a collection of database objects, (tables).
View a table's content: select * from {tablename};


Aggregate Functions:
Used to compute a single result from a set of input values.

To count the number of rows in a table: select count(*) from {tablename};


Where clause: select {column} from {tableName} where {conditons...};

LIKE works with strings only. So we need to type cast data types accordingly.

For type casting, use ::.


Rest can be better understood by watching and implementing simultaneously from the video at https://www.youtube.com/watch?v=7Hv8uhwK8qk&t=1889s
