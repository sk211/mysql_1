# mysql_1
* Databse insert

insert into tableName(
id,Name,roll,regestion,address) values (3.'sujan','5',564,feni Devipur);


*Upadte Database

update TableName set name ='sujan' where id =1


* dalete Database

dalete from tableName where id =3;

* Delete all table data command

truncate table tableName;


**multifal data insert run

Begin 

insert into Table (Id,name,roll,regestition,address) values (1,'sujan','5,56,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (2,'lition','6,57,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (3,'sanjoy','7,58,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (4,'rakib','8,59,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (5,'anik','9,60,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (6,'ayon','10,61,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (7,'rajib','11,62,Feni Debipur);
insert into Table (Id,name,roll,regestition,address) values (8,'anima','12,63,Feni Debipur);
End;


***multiful update 
update tableName set name = 'akash' where id in (1,5,8);
update tablename set gende= 'akbor' where i in (1,2,3);


***Delete mulful 

Delete from tablename where id in (1,3,9);

delete from tablename where id



 1.MAKE FORENKEY -alter table Empoloye add constraint cons_employee_fk Foreign key (GenderID) referances Gender (id)
2.DELETE FOREIGN KEY- Drop employe constraint cons_employee_fk


* Primary key:

create table EmployType(
id int not null Primary key,
Employ_name varcher(50) not null,
Employ_Address varcher (50) 
employTypeId int
);



* defautl constraint

1.alter table Employe
add constraint (constraing_name) employeeTypeIs_DefaultCons
Default 2 for EmployeeTypeId


insert into Empoyee(id,Name,Email,GenderId,) valuse (5,'a@gmail.com', 'mail')


* Cascading referential integrity constraint

** Part 10
Select record for table

	select * from tablename
		how to show fixed colume reselt

		select name from tablename

		select address from talbename

how to show fixed id ruselt

 select * from tablename whrer id =1;


** Part 11

Check constraint

Add colum ->Alter table tablename 
add columName int

show Add colum
Select * from tableName

insert data Table 

insert into tablename(
ID,name,email,age,Genderid,EmployTypeId) values(3,'sujan','a@gmail.com',1,2,-30);


add Expression or Condition

Age >0 AND Age <100


Add constriaint

Alter table tableNamea
Add Constraint ConstrainName check (Age> 0 AND AGE<100)


Delete Constraint constraintName
Drop Constrain  Emoply 


** part 12

Identity Colummm

Select * from tableName

insert into cousomer Values('sujan');

delect froem table where name/id =table id=1?


* how to set old id in new id

set indentity_insert customerName ON

Delete any Table data

->selete from tableName

how to delete hide id Number

delete table id data cmd->DBBC CHECKIDENT (TABLE_iD RESEED,0)


** Part -13

Delete and truncate

Delete->Delet any data
	Delete from tableName where (any name or id)

Truncate->
	truncate table talbeName

	-> truncate delete data in data base any id and data
	strat id 1

** Part -14
	1.last Generated row idintity
		cmd->Select SCOPE_IDENTTY()

    2.@@IDENTITY
    cmd->Select @@IDENTITY

    3.select IDEENT_CURRENT('TABLENAME')

** Part -15

   1.Unique key constraint

   cmd

   	select * from tableName

   	trsert into tableName values ('tashfiqre',123.456);

   	Alter Table Csastomer
   	Add constraint qk_coscomer_passportNO unique (PassportNo);


   	** Part -16
   	contrain summary

   	->Not null->Any colum cannot store NUll value
   	->unique-Ensure that each row for a column must have a qniqur value
   	->Primary key-
   	->Forenge key
   	_>check
   	->Default->

   	** Part -17

   	Select Statement

   	Select Specific rows
   	->select all rows
   	-Filtering with whereclause
   	->joining multiple
   	->sort rows using order by
   	select top n
   	Select top n Pecent

** part -18

sql oparator

= if the valuse of tow opa


** Part -1
create Database -> Create Database Database_name;
Delete Database -> Drop Database Databases_name;


** part -2 
Create Table 

create table Table_name(
id int not null auto_increment,
firestName varchar(255),
lastName varchar(255),
address varchar(255),
city varchar(255),
division varchar(255)
primay key(id)

);

** part -3

Data insert

1.single line data insert

insert into Table_name (firstName,lastName,address,email,city,diision)
VALUES ('sujan','majumder','Feni','sujanmajumder211@gmail.com','feni','chittagong');

2.multi line Data insert

insert into Table_name (firstName,lastName,address,email,city,diision)
VALUES 
('sujan','majumder','Feni','sujanmajumder211@gmail.com','feni','chittagong');
('akbor','Hosan','Feni','akborhosan@gmail.com','feni','chittagong');
('ayon','majumder','Feni','ayonmajumder211@gmail.com','feni','chittagong');
('anik','majumder','Feni','anikmajumder211@gmail.com','feni','chittagong');
('rajib','majumder','Feni','rajibmajumder211@gmail.com','feni','chittagong');
('rakash','majumder','Feni','rakashmajumder211@gmail.com','feni','chittagong');
('sanjoy','majumder','Feni','sanjoymajumder211@gmail.com','feni','chittagong');


** part -4

Mysql Data Update 

updata table_name  set email= 'rajib@yahoo.com' where id=2;

Risk->must use where condition 
Don't use where change all data 1 mistack

** part -5

Delete Data

delete from table_name where id =id_number;


** part -6

Alter table

->alter table table_name ADD newcol varcher(255);

-> alter table table_name
   MODDIFY COLUMN name int(11) 

 ->alter table table_name 
 DROP COLUMN  COLUMN_name

 ** part-7

select Data

->select  * from table_name
->select  * froem Table_name LIMIT 3;
>select fristName lastName;
->select * from Table_name where id=2;
select * from table_name order by lastName;
select * from tale_name ORDER By DESC;
select * from tale_name ORDER By ASC;
select cIty from table_name;
select DISTING city from table name -> don't show same data


** part -8

Sql Operators

-> = Equal To-Author ='Sujan'
-> <> NOT Equal-<> -'sales'
-> > Greater than - Hire >500
-> >= Greater than - Equal- Dependents>=2
-> < Less than -Bonus <500
-> <= Less than Equal - 
-> And
-> or
-> Between-Betwen an inclusive range-cost BETWEEn 100 and 500
->LIKE 
->IN-Equal to one of multiple possible values
->IS or IS NOT - Compare to null(missing data)
->IS NOT DISTINCT FROM - is quual to value ot both are nulls (missing data)
->AS-used to change a field name when viewing results


** part -9

BETWEEN opraton


select * from tableName where age BETWEEN 20-30;

** part -10

like oparator(for serch)

->select * from tableName where city LIKE '%r';
->select * from tableName where city LIKE 'r%';
->select * from tableName where city LIKE 'bang%';
->select * from tableName where city LIKE '%bang';
->select * from tableName where city NOT LIKE '%bang';

** part -11
in oparator (for fixed value)

for Dhaka feni
->select * from table name where dividsion in ('dhaka'.'Feni');

For Rajshahi and feni
->select * from table name where dividsion in ('Rajshahi'.'Feni');

** Part -12

sql indexes

-> create index cIndex on table_name(city )

delete index

--> drop index cindex  on table_name ;

** part -13
RElation and foreigen key

-> create table products(
id int not null auto_increment,
name varchar(255),
price int,
primary key (id)

);

-> create table order(
id int not null auto_increment,
orderNumber varchar(255),
productId int,
customerID int,
orderDate Datetime default current _timesstamp ,
primary key (id)
foregn key(productID) references productes(id)
);



** part -14

sql joins

inner jonin 
left jooin
right join
full join


* Inner jotin

join order table and product table/match colum

->select tabel_name.last name tabel_name.fires_name,  Inner join table_name.columName
from customers
inner join order on
customer.id order by 























