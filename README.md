#Create table Student 

Create table Student (
studentid char(4)  not null,
studentname varchar(20) not null,
Address varchar (20) not null,
Class varchar (10) not null,
primary key (studentid));

#create table Game

create table Game(
Gid char(4) not null,
Gname varchar(20) not null,
primary key (Gid));

#create table Student_Game 

create table Student_Game (
studentid char(4)  not null,
Gid char(4) not null,
Hours char (4) not null,
primary key (studentid,Gid),
Foreign key (studentid) References student (studentid));
