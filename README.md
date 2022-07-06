# Database-I

## Lecture requirements
--------------------
Online (paper and programming) exam at the end of the semester, in the exam period. Attendance is compulsory, it will be monitored through Microsoft Teams.              (If you have any problems, please let me know about that. I will accept what is acceptable concerning attandance.)

## Practice requirements (Group 1)
---------------------
Attendance is compulsory, it will be monitored through Microsoft Teams. If you miss more than 3 occasions you will not get a practical grade. There can be compulsory exercises during practices, and if you don't complete them, it counts as a miss. (see in db1_exercise1.txt, db1_exercise2.txt ...) There will be two tests in the semester, a midterm test (7th practice) and an endterm test (12th practice). In the tests you have to write exercises in paper (you will type it into a file) 
and write SQL and PL/SQL programs by computer. The practical grade (1-5) will be the average of the two test grades. (e.g. Test1: 3, Test2: 4, Average: 3.5, Final practical grade: 4) Retake will be in the first week of the exam period. If you retake a test then the average of the old and new grades will be your test grade. (e.g. original: 2, retake: 5 --> test grade: 3.5)


Some information about the databases we will use in practices:
=========================================================================
We have two Oracle databases, see below the connect information. When you connect to the databases from SqlDeveloper, you have to fill in the appropriate fields with the following information.

ARAMIS <br />
host: aramis.inf.elte.hu <br />
port: 1521 <br />
service_name: aramis <br />

ULLMAN                  
host: ullman.inf.elte.hu                
port: 1521
service_name: ullman

Your username is the same as your Neptun code, you will be informed about the initial password in pactical courses. You should change your Oracle password in the databases with the following SQL statement: ALTER USER my_username IDENTIFIED BY new_password;

You can use a client software -> SqlDeveloper
You can download it from my homepage: https://people.inf.elte.hu/nikovits/DB1/
The name of the file is something like sqldeveloper*.zip
You can find newer versions of SqlDeveloper, but this is perfect for us.

************************************************
New information !!!
If you are able, please install an Oracle Server Express Edition on your computer. You can download it from Oracle homepage. This way you can work on your own computer if the University database is busy or unavailable.
************************************************

!!! Attention !!!
-----------------
ELTE has a firewall, so you can connect to the databases from outside ELTE domain only with ssh tunneling see details in ssh_tunnel.pdf or ssh_SqlDeveloper.pdf.
=====================================================================================
SOME WORDS ABOUT YOUR ACCOUNTS IN THE UNIVERSITY, JUST TO MAKE THIS CLEAR !!!

You have several accounts (with passwords) for different computers or services. Let's see them.

1. caesar account (managed by the University, all students of the University have this account)
caesar.elte.hu is a cluster of Linux computers. You can use different services with this account,
e.g. WIFI, homepage, email, login to caesar.elte.hu with ssh connection, etc.
--> https://info.caesar.elte.hu/

2. Neptun account (managed by the University)
You can see your courses and results in Neptun system.

3. inf account (managed by the Faculty of Informatics, only students of the Faculty have this account)
You can login to the computers in the computer laboraties of the Faculty with this account
and you need this account to use Microsoft Teams.

4. database accounts (managed by me, only students attending some special courses have this account)
The passwords in the two databases are independent, so if you change one of them, the other will remain.
I can help you (change or reset your password) only in problems related to your database accounts and not
in problems related to the other 3 accounts.

For ssh tunneling you will need your caesar account (you will need an ssh connection to caesar.elte.hu), 
and of course your database account.

Topics (A brief overview of the semester)
=========================================

Before the 1st lecture 
----------------------
Overview of the requirements and topics of the semester, basic info about the tests (practice) and exam (lecture).
Technical information about the databases. Client software: SqlDeveloper.
Connecting to Oracle database servers. 
(db1_readme.txt)

**********************************************************************************
All the practical exercises are based on lecture slides, so review them as needed.
**********************************************************************************

#### 1st lecture
------------
Introduction, the relational data model. (UW_22_Rel_Model_Basics.pdf)
Two query languages: relational algebra and SQL.
Relational algebra operators. The basics of an SQL SELECT statement. 
Lect_01_RelAlgebra.pdf
SQL01_introduction.pdf, SQL02_select_basics.pdf, SQL03_where_condition.pdf

#### 1st practice
------------
Connecting to Oracle database servers. 
(--> ssh_tunnel.pdf and ssh_SqlDeveloper.pdf)
Connecting with SQLPLUS from pandora.inf.elte.hu (login.sql)
Running SQL statements.
(SQL01_introduction.pdf, SQL02_select_basics.pdf, SQL03_where_condition.pdf)
(db1_exercise1.txt)

#### 2nd lecture
------------
Relational algebra, pages from the Textbook. (UW_24_RelAlg.pdf)
Queries in SQL language: SELECT (Lect_02_SQL_Select.pdf, cr_drinkers.txt)
Set operators expressed in SQL. (SQL04_set_operators.pdf)
Relationship between relational algebra and SQL SELECT. 
Formal semantics of a SELECT statement.

#### 2nd practice
------------
Set operators expressed in SQL. (SQL04_set_operators.pdf)
Expressing queries in SQL and relational algebra.
(db1_exercise2.txt)

#### 3rd lecture
------------
Relations as multisets instead of sets. (UW_51_Multisets.pdf)
Extended operators of relational algebra. (UW_52_ExtRelAlg.pdf)
Lect_03_ExtRelAlg.pdf
A relational algebra calculator -> Relax (see Relax*.* files on homepage)
Aggregating functions: MIN, MAX, AVG, COUNT, SUM 
Creating groups, filtering groups in SQL (SQL06_grouping.pdf)

#### 3rd practice
------------
Oracle data types. (Oracle_datatypes.txt)
Built-in functions in Oracle SQL. (SQL05_functions.pdf, Oracle_functions.pdf)
(db1_exercise3.txt)

#### 4th lecture
------------
Creating groups, filtering groups in SQL (SQL06_grouping.pdf)
Different join syntaxes. (SQL07_join.pdf)
Complex SQL queries with subqueries. (SQL08_subquery1.pdf, SQL08_subquery2.pdf)
Relational algebra operators, summary. (db1_rel_alg_summary.pdf)

#### 4th practice
------------
MIN, MAX, AVG, COUNT, SUM functions in SQL queries.
Creating groups, filtering groups in SQL (SQL06_grouping.pdf)
Different join syntaxes (SQL07_join.pdf), subqueries (SQL08*.pdf)
(db1_exercise4.txt)

#### 5th lecture
------------
Data modification and Transactions. (Lect04_Modification.pdf, SQL09_DML.pdf)
Transactions in the Textbook (UW_66_Transactions.pdf)
Data Definition Language (DDL) statements in SQL. (SQL10_DDL.pdf, DDL_examples.pdf)
Creating Views. (SQL11_view.pdf, view_example.txt)

#### 5th practice
------------
Complex queries expressed in relational algebra, extended relational algebra and SQL.
Rewriting SQL into relational algebra and vica versa.
Computing the result of relational algebra expressions (RelaX).
(db1_exercise5a.pdf, db1_exercise5b.pdf)

#### 6th lecture
------------
Data Definition Language (DDL) statements in SQL. (SQL10_DDL.pdf, DDL_examples.pdf)
Constraints and Triggers. (Lect_05_Constr_Trigger.pdf, UW_7_Constr_Trigger.pdf)
Views and Indexes. (Lect_06_View_Index.pdf, UW_8_View_Index.pdf)
Creating Views. (SQL11_view.pdf, view_example.txt)
Some special Oracle features (Outer_join.pdf)

#### 6th practice
------------
Subqueries and Views (view_example.txt)
Modifying data within a table: Data Manipulation Language (DML) statements in SQL.
INSERT, DELETE, UPDATE (db1_exercise6_DML.txt)

#### 7th lecture
------------
A procedural language running within the database server: PL/SQL
Detailed info and examples in Oracle documentation: Oracle Database PL/SQL Language Reference
Basic elements of the language, examples. See -> PLSQL directory on homepage
https://people.inf.elte.hu/nikovits/DB1/PLSQL/
(Overview, basics, SQL_stmt, control_stmt, collection.)

#### 7th practice  --> Midterm test (March 28th)
------------
Exercise types in the test: 
relational algebra, SQL Select, Insert, Delete, Update, Built-in functions, join, grouping, aggregation, subqueries
Similar exercises as in ex. 3-4-5-6.

#### 8th lecture
------------
PL/SQL language cont. See -> PLSQL directory on homepage
https://people.inf.elte.hu/nikovits/DB1/PLSQL/
(Cursors, functions, procedures, exception handling.)

#### 8th practice
------------
Simple PL/SQL functions and procedures.
(db1_exercise7_plsql.txt)

#### 9th lecture
------------
DATALOG a logical query language. 
(UW_53_Datalog_rules.pdf, UW_54_Datalog_RA.pdf, UW_10_2_Recursion.pdf)
DATALOG query examples (Datalog_examples.pdf)
(Lect_09_Datalog.pdf, Lect_09_recursion_SQL.txt)

#### 9th practice
------------
SQL statements in PL/SQL programs. (Select, Insert, Delete, Update)
Processing the resultset of a SELECT statement: cursors.
Using a cursor for a 'WITH statement'. (pl_03_cursor.txt)
PL/SQL collections (record, array).
(db1_exercise8_plsql.txt)

#### 10th lecture
------------
Recursive Datalog programs. Expressing Datalog recursion in SQL.
DATALOG query examples (Datalog_examples.pdf, db1_SQL_recursion1.txt)
(UW_10_2_Recursion.pdf, Lect_09_Datalog.pdf, Lect_09_recursion_SQL.txt)
Another recursion type in Oracle SQL: START WITH and CONNECT BY.
(SQL_12_connect_by.pdf, db1_SQL_recursion2.txt)

#### 10th practice
-------------
Modifying tables with cursors in PL/SQL. Exception handling in PL/SQL.
(db1_exercise9_plsql.txt) 

#### 11th lecture
------------
Functional dependencies, Decompositions, Normal Forms.
Boyce-Codd Normal Form, Third Normal Form.
Chapters 3.1-3.5 from Textbook.
(Lect_11_FD.pdf cont., UW_3_DB_design.pdf)
In the exam there will be similar exercises like in Textbook !!!

#### 11th practice
-------------
Recursive queries; DATALOG-like and 'CONNECT BY' recursion.
(db1_SQL_recursion1.txt, db1_SQL_recursion2.txt)
(db1_exercise10.txt)

#### 12th lecture
-------------
Functional dependencies, Decompositions, Normal Forms cont.
Entity-Relationship modelling. (Lect_12_ER.pdf, UW_4_ER_pdf)
Summary, info about the exams. (Exam_info.pdf)

#### 12th practice --> Endterm test (May 9th) 
-------------
In the endterm test there will be only PL/SQL procedures and functions.
You have to do 2 exercises for grade 2, 3 exercises for grade 3 ... etc. 
I will take one exercise from db1_exercise7 ... db1_exercise10 on my homepage. 
So it is worth doing them all !!!
