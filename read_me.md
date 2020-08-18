# PostgreSQL
---

![Capture](https://user-images.githubusercontent.com/69482271/90494423-4f80a980-e165-11ea-81a6-043bf78aa949.PNG)



PostgreSQL, also known as Postgres, is a free and open-source relational database management system emphasizing extensibility and SQL compliance.PostgreSQL is a powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.



# Content
---
    * Dowload Process.
    * Installation Process.
    * Start PSQL with CMP/PSQL Shell.
    * Brief Explanation about various PSQL Query.



# Download Process(Windows)
---
Following is step by step process to install Postgre in Windows Machine:

__Step 1:__ At first go to this page [Download](https://www.postgresql.org/download/ "Download"). Then select Windows.

![download_first](https://user-images.githubusercontent.com/69482271/90490310-4c36ef00-e160-11ea-9913-a1fd4082519f.png)



__Step 2:__ Use __Download Installer__ to download.

![download_installer](https://user-images.githubusercontent.com/69482271/90490611-a041d380-e160-11ea-83cf-cfbf7b09ced3.png)



__Step 3:__ After that you'll see page like this.From here you have to download the version suitable for you machine.For me it's Version 13 beta.

![edb](https://user-images.githubusercontent.com/69482271/90491043-3544cc80-e161-11ea-9e43-a366ac90886b.png)





# Installation Process
---
__Step 1:__ Open the downloaded exe and Click next on the install welcome screen.

![setup1](https://user-images.githubusercontent.com/69482271/90491617-fa8f6400-e161-11ea-9554-b182e36ef64c.png)



__Step 2:__
<!--OL-->
    1.Change the Installation directory if required,else if leave it as it is.
    2.Click next.

![setup2](https://user-images.githubusercontent.com/69482271/90492123-a2a52d00-e162-11ea-9597-40d164b6f80b.png)



__Step 3:__ Click next.
 
![setup 3](https://user-images.githubusercontent.com/69482271/90492337-e5670500-e162-11ea-9866-569b99e57302.png)



__Step 4:__
   
   1. You may change the data location.
   2. Click Next.

![setup4](https://user-images.githubusercontent.com/69482271/90492429-ff084c80-e162-11ea-99dc-806c9408367b.png)



__Step 5:__
  1. Enter super user password. Make a note of it.
  2. Click Next.

![setup5](https://user-images.githubusercontent.com/69482271/90492834-6faf6900-e163-11ea-86ab-a9c21b592a20.png)



__Step 6:__
  1. Leave the port number as it is.
  2. Click next.

![setup6](https://user-images.githubusercontent.com/69482271/90492961-9b325380-e163-11ea-8466-4588d26d9c4d.png)



__Step 7:__ Click Next.

![setup7](https://user-images.githubusercontent.com/69482271/90493168-d3d22d00-e163-11ea-9a49-e182ee7153e0.png)



__Step 8:__ Click Next.

![setup 8](https://user-images.githubusercontent.com/69482271/90493287-00864480-e164-11ea-90e2-331d89022cd4.png)



__Step 9__: Once install is complete you will see the Stack Builder prompt.
   1. Uncheck that option. We will use Stack Builder   in more advance tutorials
   2. Click Finish.

![setup9](https://user-images.githubusercontent.com/69482271/90493579-59ee7380-e164-11ea-8a1c-80d180bc7606.png)



__Step 10:__ To launch Postgre go to Start Menu and search pgAdmin 4. And use it.

![setup10](https://user-images.githubusercontent.com/69482271/90493808-a3d75980-e164-11ea-8840-d52f936b92e9.png)


#  Start PSQL with CMP/PSQL Shell
---
__Step 1:__ Open command prompt or psql shell.

![cmd](https://user-images.githubusercontent.com/69482271/90497627-1b0eec80-e169-11ea-84b4-91f858f2c110.png)

__Step 2:__ After opening you will see something like this.

![cmd1](https://user-images.githubusercontent.com/69482271/90497950-835dce00-e169-11ea-9886-510fa3205cd5.png)

__Step 3:__  Now type __psql__ here ans press enter.

![cmd2](https://user-images.githubusercontent.com/69482271/90498519-4219ee00-e16a-11ea-8cea-d44b49cc2d7e.png)

__Step 4:__ Then CMD will seek the password you set at the time of installation. Type this password.(You can't see the pass when you are typing.Just type the correct password and press enter.)

![cmd3](https://user-images.githubusercontent.com/69482271/90498814-99b85980-e16a-11ea-85db-1dc839da8430.png)

__Step 5:__ After entering correct password you'll see something like this.

![cmd4](https://user-images.githubusercontent.com/69482271/90499007-d1bf9c80-e16a-11ea-8191-cf7a1d0d8c68.png)

It means you are ready to use.

#  Brief Explanation about various PSQL Query.
--- 

## Data Types
---
There are a varity of data types supported by psql.
You can check  [here](https://www.postgresql.org/docs/9.5/datatype.html "here") for all of them.

![data_types](https://user-images.githubusercontent.com/69482271/90503906-084ce580-e172-11ea-8d11-eef1407877f3.png)

## Help for using different keywords:
---
There are many keywords which'll help you during using psql command.
To use this type __help__ in you cmd.

![help](https://user-images.githubusercontent.com/69482271/90504125-68dc2280-e172-11ea-9823-84dd119ed98c.png)

Above you can see differnt key words for differnt command and help. Ex. __\q__ will quit the process and user have to use __psql__ command and give the __Password__ to re-enter.

## Create Database:
---
well,at first you have to create a database to store data and use differnt types of query or manipulation.

To create a database the psql command is:

    create database dbname;

here, dbname means database name.The user will give it as his/her wish.

I'll create a database named __test__.

![cd](https://user-images.githubusercontent.com/69482271/90504659-367ef500-e173-11ea-8d49-f0101b38f1d4.png)

If the comaand is ok and the creation of database if successfull then the message given below will be shown:

![cdr](https://user-images.githubusercontent.com/69482271/90504801-6f1ece80-e173-11ea-8b08-c9b650aeb6d9.png)

So,the only database now i have created is __test__.

## Delete Database
---
Sometimes it is necessary to delete a database. But from a greater point of view it is unwise. Cause if a database once deleted it will never be available for use. All the data will be lost. So if anyone tries to perform this command he/she must be sure about it's consequences.

To create a database the psql command is:

    drop database dbname;

Now I am deleting my database named __test__ for showing how it looks.

![dd](https://user-images.githubusercontent.com/69482271/90505364-4ea34400-e174-11ea-9d3e-9709c493eacd.png)

If the deletion is successful then the message given below will be shown:

![ddr](https://user-images.githubusercontent.com/69482271/90505460-7abec500-e174-11ea-8692-ef3f955aeefc.png)

## Connect database:
---
To insert, manipulate and retrive data you have to connect with the database. There are two ways of doing that.

### __Type 1:__ 
At first use __q__ to quit. Then type the command below:

    psql -h host_name -p port_num -U username dbname

here,

    port_num= 5432 (by default) 
    host_name= localhost (by default)
    user_name= postgres
    dbname= name of database to connect

After using this command __password__ is required. Then you are connected to your desired database.

![connect1](https://user-images.githubusercontent.com/69482271/90506176-a9896b00-e175-11ea-9c01-8312ea25ccf9.png)

### __Type 2:__
This is more easy.You have to just use __\c__ keyword to connect. In this case no need to quit. But in first type we had to quit.

    \c dbname

![connect2](https://user-images.githubusercontent.com/69482271/90506573-52d06100-e176-11ea-98e9-28408df3ada0.png)

See! Easy to connect.

## Create Table
---
Now we'll see how to create a table in a database. In a database the data/info are stored using tabular form.So it is very important to know how to create a table in psql.

Command to create a table:

    CREATE TABLE table_name(
     column1 datatype,
     column2 datatype,
     column3 datatype,
     .....
     columnN datatype,
);

Now I will create a table named __mock1__. It is bascically a table of a data of different persons.

![ct](https://user-images.githubusercontent.com/69482271/90507186-4993c400-e177-11ea-9d2a-f27965948257.png)

Explanation:

    1. Here columns are id,first_name,last_name, email, date_of birth,birth_country.
    2. bigserial= It is a datatype wich sequentially increment the iterator/int.
    3. varchar(x)= varchar is a string of length x.
    4. date= to use date as a column we have to use the datatype date.

If the creation of tabke is done, then the message giveb below will be shown:

![ctr](https://user-images.githubusercontent.com/69482271/90507636-07b74d80-e178-11ea-96c6-bb158a4087f9.png)

## Describe Table:
---
To see the table structure or to simply to describe the table use __\d__ keyword.
    
    \d table_name;

Let's see how my table __mock1__ looks like:

![dt](https://user-images.githubusercontent.com/69482271/90508271-3b46a780-e179-11ea-86f8-aaaf723eaca9.png)

## Drop Table
---
Same as delete a database one should be causious when deleting a table.Cause once it is deleted there is no way the deleted data can be retrived.

Command:
    
    drop table table_name;

Now I m deleting the table mock1 to see how it looks:

![dltt](https://user-images.githubusercontent.com/69482271/90508475-a1cbc580-e179-11ea-84ef-e82152a08832.png)

If is successful then the message below will be shown:

![dlttr](https://user-images.githubusercontent.com/69482271/90508610-de97bc80-e179-11ea-8893-dcb77fe5bd3c.png)

## Create Table with Constraints
---
Now I'll again create a table, but this time with constraints. Constraints plays a vital role. It is a must for a good database management system. Without constraints it can be said that the database is of no use if practical life.

Command:

    CREATE TABLE table_name(
     column1 datatype  constraints(optinal),
     column2 datatype  constraints(optinal),
     column3 datatype  constraints(optinal),
     .....
     columnN datatype  constraints(optinal),
);

Now I am creating __mock1__ again with constraints.

![ctc](https://user-images.githubusercontent.com/69482271/90509053-9036ed80-e17a-11ea-988c-43a040f9500a.png)

Let's Describe this table now and see what it looks like now:

![dtc](https://user-images.githubusercontent.com/69482271/90509215-c83e3080-e17a-11ea-967c-ae321ef87960.png)

If you take a close look then you can see there are __not null__ indicating the value of this column can not be null. And also there is __mock1_pkey__ as primary key.






