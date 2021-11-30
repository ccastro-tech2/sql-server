# sql-server

Introduction
 
Backup package (BACPAC) contains schema and data for SQL Server database. We can export the database into BACPAC and import it in new environment as a new database. This can be used as per our convenience to migrate data from one environment to another or one SQL Version to another. This restore option has become best choice for Database Administrator and developer for migration or restore database for various purposes.
 
This article describes how to import BACPAC file using SQL Server Management Studio. In this example, I have used SQL Server 2019 Developer edition and I would
recommend to use latest version of SQL.
 
Let us go to import options. In the example, I will use already created BACPAC file. If you don’t have file and need assistance to create BACPAC file, you can go through my previous article on How to Export BACPAC.
 
Steps to Import/Restore BACPAC file
 
Step 1
 
Open SQL Server management studio, connect to SQL instances where you want to restore database and right click on Database. Then you will get option as shown in below picture. Click on Import Data-tier Application.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Step 2
 
You will get below window. Click on Next as illustrated in below picture.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Step 3
 
Then, you will get option to import backpack file either from Local disk or from Windows Azure. As I am explaining the steps to import backpack file from local storage file, we will select Import from Local disk option and browse the file in this step.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
However, we can connect to Azure Storage account and import file from Storage account and create new database with that file.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
To import from Windows Azure, once we click connect Option, we have to Sign in with Azure account and select the Storage Account, Blob container and click on OK.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
As the focus of the article is to import from local disk. Let’s continue with Local file import steps.
 
Import the file from local Disk and click on Next.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Step 4
 
Give the name of your Database and click on Next. You can keep default file path for the Data and Log. However, you can change, file path for Data and Log.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Step 5
 
In this step, detailed summary of your previous selections will be seen as depicted below. Click on Finish to proceed further.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Step 6
 
Once you click on Finish, it starts creating database, based on your BACPAC file.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
It may take few minutes to create database, tables, stored procedure, Views etc. and import data to the tables. Wait for process to complete.
 
How To Import Or Restore BACPAC File Using SQL Server Management Studio
 
Once it is completed, you can see what are the tables, store procedures, views so on created on the result windows as well as you will get option Close, click on Close.
 
Now, database is created using BACPAC file. You can check and verify your database. It is ready to use as per your need.
 
Conclusion
 
In short, this article has described how to create database using BACPAC file. I hope, article helps developer and database administrator to create database from one environment to another by using SSMS and importing database BACPAC file.
