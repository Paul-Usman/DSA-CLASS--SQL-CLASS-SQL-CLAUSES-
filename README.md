# DSA-CLASS--SQL-CLASS
This is where I review some of the queries used SQL classes.

## Table of Contents
- [Project Overview](#Project-Overview)
- [Data Sources](#Data-Sources)
- [Tool Used](#Tool-Used)
- [Explorative Data Analysis](#Explorative-Data-Analysis)
- [Data Analysis](#Data-Analysis)
- [Result/Findings](#Result/Findings)
- [Recommendations](#Recommendations)
- [Limitations](#Limitations)
## Project Overview.
In this project, I will do well to chronicle all the commands and analysis done the class. The structured query language uses simple every day English terms, however, for analysis some commands had to be used to display the needed results.

### Data Sources.
Most of the data for SQL are imported, however some queries will be written out here to show how some table are created.
### Tool Used.
- Ms SSMS [Download Here](https://aka.ms/ssms/21/release/vs_SSMS.exe)
### Data Analysis.
Here are some queries for creating tables;

``` SQL
create table Employee(
Staffid varchar (10),
FirstName varchar (100),
LastName varchar (100),
Gender nvarchar (10),
Date_of_Birth date,
HireDate date,
primary key (staffid)
)
INSERT INTO Employee(Staffid, Firstname, LastName, Gender, Date_of_Birth, HireDate)
Values ('IM201','Thoby','Elumelu','male','1995-06-24','2020-02-03')
CREATE TABLE Salary(
salary_id int identity (1,1) not null,
Staffid varchar (255),
FirstName varchar (255),
lastname varchar (255),
department nvarchar (max),
salary decimal (10, 3)
)
INSERT INTO salary (Staffid, Firstname, LastName, department, salary)
Values ('IM201','Thoby','Elumelu','Tech','150000.9786')
