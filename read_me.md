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

## Insert Into Table:
Now we'll see how to insert a entity or row in a table. It is obvious that without insert data there is nothing we can do.

Command:

    INSERT INTO TABLE_NAME (column1, column2, column3,...columnN)
    VALUES (value1, value2, value3,...valueN);

Explanation:

* Here, column1, column2,...columnN are the names of the columns in the table into which you want to insert data.
* The target column names can be listed in any order. The values supplied by the VALUES clause or query are associated with the explicit or implicit column list left-to-right.

Now lets see how it looks to insert into mock1.

![it](https://user-images.githubusercontent.com/69482271/90516669-26bcdc00-e186-11ea-92ee-04ec6a9bf8f9.png)

If insertion is successful then the message given below will be shown:

![itr](https://user-images.githubusercontent.com/69482271/90516772-494ef500-e186-11ea-90a2-d4ae73db8ded.png)


## Generate rows using MOCKAROO
---
Using [Mockaroo](https://www.postgresql.org/download/ "Mockaroo")  we can generate upto 1000 rows at a time.  At first visit the given link.

__Step 1:__ Create the columns and specify the data types.There are all available option to do this.

![mro](https://user-images.githubusercontent.com/69482271/90516808-58ce3e00-e186-11ea-9335-6b256becac75.png)

__Step 2:__ 

* Change the file format to SQL.
* mark the __include create table__ box.
* Download.

![mro1](https://user-images.githubusercontent.com/69482271/90516892-769ba300-e186-11ea-9b75-0e411d40f5db.png)

__Step 3:__ Now we have to add constraints. To do this I have used VSCODE.

* Open the file with VSCODE.
* Change the necessary things and add constraints.
* save.

Two pictures are given below:

* without adding constraints and without any change.

![vsc](https://user-images.githubusercontent.com/69482271/90518113-23c2eb00-e188-11ea-8bfa-3f36f7cd8baa.png)

* with necessary change.

![VSC1](https://user-images.githubusercontent.com/69482271/90518123-26bddb80-e188-11ea-9563-d3e6414405cc.PNG)

Now we have insert this table.There is a nice way to do this. At first lets do somethig.

Type this command:
 
    \?

![see](https://user-images.githubusercontent.com/69482271/90518727-f6c30800-e188-11ea-988f-4419197a27da.PNG)

Here we can see __\i__ command. By using this we can easily add the table in database.

Command:

    \i path_of_the_file;

![ict](https://user-images.githubusercontent.com/69482271/90520056-ac428b00-e18a-11ea-9f88-f7642bfbe394.png)


Thus we can easily make table.

## SELECT
---

PostgreSQL SELECT statement is used to fetch the data from a database table, which returns data in the form of result table. These result tables are called result-sets.

Command:
     
     SELECT column1, column2, columnN FROM table_name;
We can use a __asterisk(*)__ to show all the collumns.

Lets fetch data from Mock1 table.

* We'll see all the column by using a   __(*)__.
![sel](https://user-images.githubusercontent.com/69482271/90520935-c6309d80-e18b-11ea-8bb0-9ffabdcd8439.png)

* We can specify tables. In this case we only see 3 columns(id,first_name,last_name).
![sel1](https://user-images.githubusercontent.com/69482271/90520942-c7fa6100-e18b-11ea-8cb4-73e765b87c33.png)

## Order by(Sort):
---
Sometimes it is need to rearrage the table in accending or decending order in respect of a column or multiple columns. To do so we can use __order by__.

Command:

    SELECT column-list
    FROM table_name
    [WHERE condition](OPTONAL)
    [ORDER BY column1, column2, .. columnN] [ASC | DESC];

We can rearrange the table both in accending and decending order.

__Accending Order:__ To rearrange the table in accending order we use __ASC__ or __nothing at all__ after __ORDER BY__.

1. Order by id:
![ord](https://user-images.githubusercontent.com/69482271/90521993-03495f80-e18d-11ea-9958-b8bd9abf020d.png)

1. Order by first_name:
![ord](https://user-images.githubusercontent.com/69482271/90522148-30960d80-e18d-11ea-8443-03e64a13d4af.png)

__Decending order:__
To rearrange the table in accending order we use __DESC__ after __ORDER BY__.

1. Order by id:
![ord2](https://user-images.githubusercontent.com/69482271/90522411-7d79e400-e18d-11ea-8972-48562f7d6c8e.png)

1. Order by first_name:
![ord3](https://user-images.githubusercontent.com/69482271/90522419-7fdc3e00-e18d-11ea-9511-d9f84248821b.png)

## Dintict:
---
The PostgreSQL DISTINCT keyword is used in conjunction with SELECT statement to eliminate all the duplicate records and fetching only unique records.

There may be a situation when you have multiple duplicate records in a table. While fetching such records, it makes more sense to fetch only unique records instead of fetching duplicate records.

Coomand:

    SELECT DISTINCT column1, column2,.....columnN
    FROM table_name
    WHERE [condition]

Lets see only the countries without using distinct:
![dis2](https://user-images.githubusercontent.com/69482271/90523175-64bdfe00-e18e-11ea-8bd4-0b37d585bd8a.PNG)

Now if we use distinct then we can see the duplicate data will be removed.

![dis](https://user-images.githubusercontent.com/69482271/90523158-625ba400-e18e-11ea-909d-63d75cf145fe.png)

## Where Clause
---

The PostgreSQL WHERE clause is used to specify a condition while fetching the data from single table or joining with multiple tables.

If the given condition is satisfied, only then it returns specific value from the table.

Command:

    SELECT column1, column2, columnN
    FROM table_name
    WHERE [search_condition];

Lets find out the details of this person who has a id=101.

![whe](https://user-images.githubusercontent.com/69482271/90523784-1b21e300-e18f-11ea-8591-5df577fa5b36.png)

Now suppose we know the first name to find the entity.

![whe1](https://user-images.githubusercontent.com/69482271/90523793-1c531000-e18f-11ea-82fa-3d2a5678c511.png)

N.B. If we use primary key as condition then we always get 1 entity. But otherwise it is possible to get multiple rows.

## Limit, Offset and Fetch
---
__Limit:__ By using limit we can tell how many rows we want from the starting. Suppose we wan't to know the details of the first X rows.Then we should use limit.

Command:

    SELECT COL1,COL2..COLN FROM TABLE_NAME LIMIT X;

Lets see the first 10 rows of mock1.

![limit](https://user-images.githubusercontent.com/69482271/90524664-29243380-e190-11ea-8b1a-04293c43bf01.PNG)

__Offset:__ If we want to ignore the first X rows and start to know the detail after the Xth row, Then we use offset.

Command:

    SELECT COL1,COL2..COLN FROM TABLE_NAME OFFSET X;

Suppose we want to know the 11th to 20th row.

![offset](https://user-images.githubusercontent.com/69482271/90524675-2cb7ba80-e190-11ea-8777-5c19df69d345.PNG)

__Fetch__: Constrains the maximum number of rows returned by a statement or subquery. Both LIMIT (Postgres syntax) and FETCH (ANSI syntax) are supported, and produce the same result.

Command:

    SELECT COL1,COL2..COLN FROM TABLE_NAME FETCH FIRST X ROWS ONLY;

![fetch](https://user-images.githubusercontent.com/69482271/90524689-304b4180-e190-11ea-9738-2eb74bd85e70.PNG)

## Between
---
The BETWEEN operator selects values within a given range. The values can be numbers, text, or dates.

The BETWEEN operator is inclusive: begin and end values are included. 

Command:

    SELECT column_name(s)
    FROM table_name
    WHERE column_name BETWEEN value1 AND value2;

If we want to see the data between id 100 and 110.

![bet](https://user-images.githubusercontent.com/69482271/90526756-989b2280-e192-11ea-9249-8b627c975bbd.png)

## In Operator
---
The IN operator allows you to specify multiple values in a WHERE clause.

The IN operator is a shorthand for multiple OR conditions.

Command:

    SELECT column_name(s)
    FROM table_name
    WHERE column_name IN (value1, value2, ...);

Suppose we want to know the entity which birth_country is either __Bangladesh__ or __Australia__ or __Nigeria__.

![in](https://user-images.githubusercontent.com/69482271/90527278-2ecf4880-e193-11ea-90ce-9b25aab8dc27.PNG)

## Like and Ilike
---
The PostgreSQL LIKE operator is used to match text values against a pattern using wildcards.

![wild](https://user-images.githubusercontent.com/69482271/90527858-d482b780-e193-11ea-82fc-9f10988f027d.png)

 If the search expression can be matched to the pattern expression, the LIKE operator will return true, which is 1.

There are two wildcards used in conjunction with the LIKE operator −

1. The percent sign (%)

1. The underscore (_)

The percent sign represents zero, one, or multiple numbers or characters. The underscore represents a single number or character. These symbols can be used in combinations.

    SELECT FROM table_name
    WHERE column LIKE 'Desired Expression';

Suppose we want all the entity with email starting with a letter _a_.

![like](https://user-images.githubusercontent.com/69482271/90528377-5bd02b00-e194-11ea-97fc-e5bd33496146.png)

The ILIKE operator do the same as like except Ilike is case insensative. Means, '%a%' and '%A%' are not same for like but both are same for Ilike.


    






