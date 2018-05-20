# Sqoop
sample sqoop script


Sqoop = Sql + Hadoop   
SQL import export utility. 
Sqoop is an open source software product developed by the Apache Software Foundation.
•	Sqoop is a command-line interface application for transferring data between relational databases and hadoop.
•	Sqoop works with relational databases such as Teradata, Netezza, Oracle, MySQL, Postgres, and HSQLDB.
•	You can use Sqoop to import data from a relational database management system (RDBMS and Data Warehouses) such as MySQL or oracle into Hadoop Distributed File System (HDFS), transform the data in Hadoop MapReduce, and then export the data back into RDBMS.
•	Sqoop uses MapReduce to import and export the data, which provides parallel processing.
•	It is used for integration.
•	Sqoop import/export goes with only mapper not reducer jobs.
•	Sqoop by default launches 4 no of mappers.
Usage
With Sqoop you can import data from a relational database system into HDFS.
The input to the import process is a database table.
Sqoop reads the table row-by-row into HDFS.
The output of this import process is a set of files containing a copy of the imported table.
The import process is performed in Parallel For this reason, the output will be in multiple files.
IN REAL TIME PROJECTS WE ARE NOT AUTHORIZED TO CONNECT TO DATABASES (RDBMS) (upstream)
WE MUST IMPORT/EXPORT DATA ONLY THROUGH SQOOP
WE CANNOT GIVE EXPLICIT CONNECTIONS LIKE     sudo mysql;
Declaration
sqoop          list-databases   --connect jdbc:mysql://localhost --username root

Sqoop                                   is the Keyword                                        
list-databases                          is the Action Qualifier
--connect jdbc:mysql://localhost        is the connection URL  
--username                              is the username
--password                              is the password (if prompted)
                                                                             

Here jdbc is a driver
Here we are not mentioning the password because we are going with root user. So, we don’t mention the password.
