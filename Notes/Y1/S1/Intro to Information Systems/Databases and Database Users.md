# Database and Database Users

``` traditional database applications ``` are like CRUD applications
``` modern database systems ``` referred to as big data
``` NOSQL ``` e.g. MongoDB are databases with no consistent structure to uphold
``` cloud storage ``` whereby users are prodivded with storage capabilities on the Web for managing all types of data
``` multimedia databases ``` store sensory files, images, audio, video
``` Geographic information Systems (GIS)``` store and analyze maps, weather data, and satelittle
``` Data Warehouses ``` and ``` online analytical processing (OLAP) systems ``` are used in many companies to extract and analyzed useful business information from very large databases 
``` Real-time ``` and ``` active database technology ``` are used to control industrial and manufacturing processes
``` search techniques ``` are applied to the WWW to improve search

# 1.1 Intro

A ``` database ``` is a collection of related data. They can be any size and complexity
``` data ``` are known facts that can be recorded and that have implicit meaning

## Case Study of Amazon
Amazon.com holds data for over 60 million active users, 1M of books, CDs, videos, DVDs, games, electronics, etc. 
The DB occupies over 42 TB

``` database management system (DBMS) ``` is a computerized system that enables users to create and maintain a database
``` Protection ``` includes system protection against hardware or software malfunction 
#### Do backups count as protection or just safety precaution ?
and `` security protection `` against unauthorized or malicious access

### Design Process
1. Requirements Specification and analysis
2. Conceptual design
3. Logical design
4. Physical design

## 1.3 Characterisits of the Database Approach
``` file processing ``` where each user defines and implements the files needed for software 

### 1.3.1 Self-desecribing Nature of a Database System
``` meta-data ``` describes the structure of the primary database
``` self-describing data ``` that inclues the data item names and data values in one structure

### 1.3.2 Insulation between Programs and Data and Data Abstraction
The ability to seperately store of the structure of data files in the DBMS catalog 
is called ``` program-data-independence ```

For example, a file access program may be written in such a way that it can access
only STUDENT records of the structure shown in Figure 1.4. If we want to add
another piece of data to each STUDENT record, say the Birth_date, such a program
will no longer work and must be changed. By contrast, in a DBMS environment, we
only need to change the description of STUDENT records in the catalog (Figure 1.3)
to reflect the inclusion of the new data item Birth_date; no programs are changed.
The next time a DBMS program refers to the catalog, the new structure of
STUDENT records will be accessed and used.

OO and OR systems allow users to define operations on data as part of the database
definition. This is called an operation which is specified in two parts `interface`,
the operation name and data types of its arguments, `implementation` the action.
This behaviour is called `program-operation independence`

the characteristic that allows program-data independence and program-operation 
independence is called `data abstraction`.

``data models`` are a type of data abstraction that is ued to provide representation
by only showing the data it hides storage and implementation details

### 1.3.4 Sharing of Data and Mutliuser Transactions
``multiuser DBMS`` allow mutiple users to access the database at the same time
the DBMS must include `concurrency control` to ensrue that several users updating 
data do so in a controlled manner 

## 1.4 Actors
### 1.4.1 Admins
``Database admins (DBA)`` are repossible for administering these resources, and auth-
orizing access to the database, coordinating and monitoring its use

### 1.4.2 Database Designers
``Database Designers`` are responsible for identifying the data and structure of it 
to be stored. They interview and ask prospective database users

### 1.4.3 End Users
``End Users`` are the people whose jobs require access to the database

``canned transactions`` are standard types of queries and updates

Types of End Users:
1. `Casual users` occasinally access the DB
2. `Naive users` constantly query and update the DB using canned transactions
3. `Sophisticated users` familiarize themselves with the DBMS to implement their 
    own applications
4. Standalone Users maintain personal DBs by using ready-made programs

### 1.4.4 System Analyst

`System analysts` determine the requirements of end users, particularly naive and
parametric end users 

`Application programmers` implement these specification as programs

## 1.5 Workers
`modules` are implementation for CRUD features

## 1.6 Advantages of Using DBMS approach
### 1.6.1 Controlling Redundancy
`redundancy` are useless/unnecessary ways of storing and manipulating data
`data normalization` enesures consistency and save storages through storing objects 
in one place
`controlled redundancy` improves performance of queries by denormalization

### 1.6.2 Restricting Unauthorized Access
DMBS should provide a `security and auth subsystem`

### 1.6.3 Providing Persistent Storage for Program Objects

