# II-CSE-E-SEC-DBMS-LAB
DBMS LAB FOR AY 2026-27 I SEM
##CREATE TABLES OF DATABASE WITHOUT CONSTRAINTS
```
CREATE TABLE student(
    name  VARCHAR2(30),
    student_number NUMBER,
    class  NUMBER,
    major VARCHAR2(20)
);
CREATE TABLE course (
    course_name   VARCHAR2(30),
    course_number NUMBER,
    credit_hours  NUMBER,
    department    VARCHAR2(30)
);
CREATE TABLE section1 (
    section_identifier NUMBER,
    course_number      NUMBER,
    semester           VARCHAR2(30),
    year               NUMBER,
    instructor         VARCHAR2(30)
);
CREATE TABLE grade_report (
    student_number     NUMBER,
    section_identifier NUMBER,
    grade              VARCHAR2(30)
);

##INSIDE VALUES INSIDE THE TABLE
INSERT INTO student VALUES ( 'sai',17,1,'cs' );
INSERT INTO student VALUES ( 'ram',23,1,'cs' );
INSERT INTO student VALUES ( 'jaylor',16, 1, 'cs' );

INSERT INTO course VALUES ( 'MATH',102,3, 'cs' );
INSERT INTO course VALUES ( 'python',104,3,'cs' );

INSERT INTO section1 VALUES ( 34,303,'fail',3, 'jaylor' );
INSERT INTO section1 VALUES ( 35,304,'pass',3,'rathod' );
INSERT INTO section1 VALUES ( 34,305,'fail', 3, 'resur' );

INSERT INTO grade_report VALUES ( 34,303,'A' );
INSERT INTO grade_report VALUES ( 34, 303, 'B' );

##DESCRIBE ALL TABLES 
DESC student;
DESC course;
DESC section1;
DESC grade_report;

##LIST THE CREATED TABLES
SELECT *FROM student;
SELECT *FROM course;
SELECT *FROM section1;
SELECT *FROM grade_report;

##DISPLAY THE VALUES OF EACH TABLE
SELECT *FROM student;
SELECT *FROM course;
SELECT *FROM section1;
SELECT *FROM grade_report;

##DELETE ALL TABLES
DROP TABLE student;
DROP TABLE course;
DROP TABLE section1;
DROP TABLE grade_report;
```
