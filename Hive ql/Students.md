create table StudentDetails(RollNo int, Name string, Address string,Class int);

create table StudentPerformance(RollNo int, Sub1_marks int, Sub2_marks, Sub3_marks, Percentage float);

create external table Teacher(empid int,name string, dept string);

alter table Teacher to TeacherInfo;

load data local inpath 'Path of csv' in to table StudentPerformance

select * from StudentPerformance where Percentage>60;

