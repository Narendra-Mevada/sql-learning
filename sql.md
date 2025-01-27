***Create Dtabase:***<br>
for creating Database we have to write a query like:<br>
```sql
create database database_name;
```
if we add 'if not exist' in create db query then it check is there any database whose name is same, if yes than it wouldn't create db.<br>
```sql
create database if not exists database_name;
```
---
***Delete Dtabase:***<br>
for Deleting Database we have to write a query like:<br>
```sql
drop database database_name;
```
if we add 'if exists' in drop db query than it checks there is exist any datbase which name is .... than delete it if not, than don't do.<br>
```sql
drop database if exists database_name;
```
---
***Use Dtabase:***<br>
With the help of it we can use database, after write "USE" query next all query is apply on current database.<br>
```sql
use database_name;
```
---

***Cretate Table:***<br>
We store data in table formate in Data base,<br>
For creating table and adding column we write query like this:<br>
```sql
create table table_name(
    column_1 data_type constarin,
    column_2 data_type constarin,
    column_1 data_type constarin
    );
```
for example:
```sql
create table students(
    id int primary key,
    name varchar(50),
    age int not null
    );
```
---
***Insert Data:***<br>
For inserting data into table we write query like this (we use exaple as "student" table ):<br>
```sql
insert into students (id,name,age)
values
(01,'Narendra Mevada',18),
(02,'Ankit Mevada',19),
(03,'Karan Mevada',20);

```
---
***Print Table:***<br>
Print or execute table using this query:<br>
for printing whole table:<br>
```sql
select * from students;
```
for specific column or row:<br>
```sql
select id
from students
where id=02;
```
---
***Update Data:***<br>
for update data in existing table we write query like this:<br>
```sql
update students
set name='Vishal Mevada'
where id=03;
```
---
***Delete Data:***<br>
for Delete data in existing table we write query like this:<br>
```sql
delete from students
where id=02;
```
---
---
***Types of SQL commands***<br>
1. **DDL**: Data Definition Language:<br>(Create, Altre, Rename, Trunkate and Drop).
2. **DQL**: Data Query Language:<br>(Select).
3. **DML**: Data Manipulation Language:<br>(Insert, Update and Delete).
4. **DCL**: Data Control Language:<br>(Grant and Revoke permission to users).
5. **TCL**: Transaction Control Language:<br>(Start Transaction, Commit, Rollback).<br>
---
---
***Keys***:<br>
1. **Primary Keys**:<br>It is a column (or set of columns) in a table that uniquely identifies each row.(a unique id).<br>There is only PK & it should be NOT null.
2. **Foreign Keys**:<br>Foreign key is a column (or set of colums) in a table that reffers to the Primary key of another Table.<br>There can be multiple FKs.<br>FKs can have duplicate & null values.