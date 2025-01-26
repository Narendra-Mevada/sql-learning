***Create Dtabase:***<br>
for creating Database we have to write a query like:<br>
```sql
create database database_name;
```
---
***Delete Dtabase:***<br>
for Deleting Database we have to write a query like:<br>
```sql
drop database database_name;
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
