# Course #4: Databases and SQL for Data Science with Python

<p align="Center">
<img src = https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/databases-and-sql-for-data-science.png>
</p>

## About this Course
This course covers SQL (Structured Query Language), which is still the most widely used query language to access databases. Also covered in this course was learning how to access the IBM db2 database using Python. Here are the topics that were covered in the course:
- Foundation SQL statements like: SELECT, INSERT, UPDATE, DELETE
- Filter result set, using WHERE, COUNT, DISTINCT, and LIMIT clauses
- Differentiate between Data Manipulation Language (DML) and Data Definition language (DDL).
- CREATE, ALTER, DROP and LOAD tables
- Use string patterns and ranges: ORDER and GROUP result setts and built-in database functions
- Build sub-queries and query data from multiple tables
- Access databases as a Data Scientist using Jupyter Notebooks with SQL and Python
- Work with advanced concepts like Stored Procedures, Views, ACID Transactions, Inner & Outer queries (**HONORS** track).

**NOTE:** The HONORS track (Week 6 Module) is completely optional for completing the IBM Data Scientist Professional Certificate program. However, this module is required in the IBM Data Engineering Track. Students who completed the HONORS track in the IBM Data Scientist Professional Certificate receive an HONORS recognition on the course certificate

To see the HONORS recognition that I receive in this course certificate, you can access the certificate with HONORS recognition **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/IBM%20Databases%20and%20SQL%20for%20Data%20Science%20with%20Python%20(with%20HONORS)%20certificate.pdf)</u>**

## Projects
The following two projects completed in this course involved 3 datasets for the city of Chicago obtained from the City of Chicago Data Portal. The following datasets used to work on **both** the two projects are as follows:

1. [Socioeconomic Indicators in Chicago](https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)
2. [Chicago Public Schools](https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)
3. [Chicago Crime Data](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)

### Installation instructions:
**NOTE:** The installation instructions for all two projects are the same &#10071;

### Step 1: Download the following datasets

**NOTE:** The datasets provided below were reduced to only 500 rows. The original datasets are over 1.55GB in size and were 6.5 million rows. Those datasets that were analyzed in the projects are stored as .CSV (comma separated values) file formats. Click on the links below to download those datasets and save them for analysis

####  1. Chicago Socioeconomic Indicators

This dataset contains a selection of six socioeconomic indicators of public health significance and a hardship index, by Chicago community area, for the years 2008 – 2012.

Here is the link to the dataset used for both projects: [Chicago Census Data](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/ChicagoCensusData.csv)


#### 2. Chicago Public Schools

This dataset shows all school level performance data used to create CPS School Report Cards for the 2011-2012 school year.

Here is the link to the dataset used for both projects: [Chicago Public Schools](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/ChicagoPublicSchools.csv)

#### 3. Chicago Crime Data

This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that occurred in the City of Chicago from 2001 to present, minus the most recent seven days.

Here is the link to the dataset used for both projects: [Chicago Crime Data](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/ChicagoCrimeData.csv)

**NOTE:** For learners who are encountering issues with loading from .csv files in DB2 on Firefox, the following datasets can be downloaded here (stored as .txt files).

1. [Census Data](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoCensusData.txt?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)
2. [Chicago Public Schools](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoPublicSchools.txt?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)
3. [Chicago Crime Data](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoCrimeData.txt?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)

### Step #2: Store the datasets in database tables

The datasets need to first be stored in the database to analyze the data using SQL.

To activate a trial with IBM Cloud Feature, you can click [here](https://reward.skills.network/claim)

For directions on how to create Db2 service instance and get started with the Db2 console, click on the link [here](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20Sign%20up%20for%20IBM%20Cloud%20-%20Create%20Db2%20service%20instance%20-%20Get%20started%20with%20the%20Db2%20console/instructional-labs.md.html?origin=www.coursera.org)

It is **highly recommended to manually load each table using the database console LOAD tool**&#10071;&#10071;

<img src = "https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/images/LoadingData.png">

##### Now open the Db2 console, open the LOAD tool, Select / Drag the .CSV file for the first dataset, Next create a New Table, and then follow the steps on-screen instructions to load the data. Name the new tables as follows:

1.  **CENSUS_DATA**
2.  **CHICAGO_PUBLIC_SCHOOLS**
3.  **CHICAGO_CRIME_DATA**

### Step 3: Connect to the databases

To establish connection with the database, first load the SQL extension

The following required modules are pre-installed in the Skills Network Labs environment. However if you run this notebook commands in a different Jupyter environment (e.g. Watson Studio or Anaconda) you may need to install these libraries by removing the `#` sign before `!pip` in the code cell below.

```
# These libraries are pre-installed in SN Labs. If running in another environment please uncomment lines below to install them:
# !pip install --force-reinstall ibm_db==3.1.0 ibm_db_sa==0.3.3
# Ensure we don't load_ext with sqlalchemy>=1.4 (incompadible)
# !pip uninstall sqlalchemy==1.4 -y && pip install sqlalchemy==1.3.24
# !pip install ipython-sql
```
```
%load_ext sql  #Load sql extension
```
In the next cell, enter your db2 connection string. From you rD2 service credentials, copy everything after db2:// (except the double quote at the end) and paste it in the cell below after ibm_db_sa://

<img src ="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/images/details.png">

```
# Remember the connection string is of the format:
# %sql ibm_db_sa://my-username:my-password@my-hostname:my-port/my-db-name?security=SSL
# Enter the connection string for your Db2 on Cloud database instance below

%sql ibm_db_sa://my-username:my-password@my-hostname:my-port/my-db-name?security=SSL
```

### Project #1: Analyzing City of Chicago Data by writing Basic SQL queries
This project contains the following SQL queries that answers the following questions:
- **Problem 1:** Find the total number of crimes recorded in the CRIME table.
- **Problem 2:** List community areas with per capita income less than 11000.
- **Problem 3:** List all case numbers for crimes  involving minors?(children are not considered minors for the purposes of crime analysis)
- **Problem 4:** List all kidnapping crimes involving a child?
- **Problem 5:** What kinds of crimes were recorded at schools?
- **Problem 6:** List the average safety score for each type of school.
- **Problem 7:** List 5 community areas with highest % of households below poverty line
- **Problem 8:** Which community area is most crime prone?
- **Problem 9:** Use a sub-query to find the name of the community area with highest hardship index
- **Problem 10:** Use a sub-query to determine the Community Area Name with most number of crimes?

To view all the SQL queries that answers all the problems, <u>**[click here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%205%20Project%20Assessment/Week%205%20Project%20Assessment%20Notebook.ipynb)**</u> to access the Jupyter Notebook&#10071;
### Project #2: Analyzing City of Chicago Data by writing Advanced SQL queries

This project contains the following SQL queries that answers the following questions, using transactions, views, joins, and stored procedures:

#### Exercise 1: Using Joins
You have been asked to produce some reports about the communities and crimes in the Chicago area. You will need to use SQL join queries to access the data stored across multiple tables.
- **Question 1:** Write and execute a SQL query to list the school names, community names and average attendance for communities with a hardship index of 98. <br><br>
The screenshot for this question can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%201.JPG)</u>**

- **Question 2:** Write and execute a SQL query to list all crimes that took place at a school. Include case number, crime type and community name.
<br> <br>The screenshot for this question can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%202.JPG)</u>**

#### Exercise 2: Creating a View
For privacy reasons, you have been asked to create a view that enables users to select just the school name and the icon fields from the CHICAGO_PUBLIC_SCHOOLS table. By providing a view, you can ensure that users cannot see the actual scores given to a school, just the icon associated with their score. You should define new names for the view columns to obscure the use of scores and icons in the original table.
- **Question 1:** Write and execute a SQL statement to create a view showing the columns listed in the following table, with new column names as shown in the second column.
  - Write and execute a SQL statement that returns all of the columns from the view.
  - Write and execute a SQL statement that returns just the school name and leaders rating from the view.
<br><br>
The screenshot for this question can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%203.JPG)</u>**

**Column name in CHICAGO_PUBLIC_SCHOOLS**| **Column name in view**
:---|:---|
NAME_OF_SCHOOL|School_Name
Safety_Icon|Safety_Rating
Family_Involvement_Icon|Family_Rating
Environment_Icon|Environment_Rating
Instruction_Icon|Instruction_Rating
Leaders_Icon|Leaders_Rating
Teachers_Icon|Teachers_Rating

#### Exercise 3: Creating a Stored Procedure
The icon fields are calculated based on the value in the corresponding score field. You need to make sure that when a score field is updated, the icon field is updated too. To do this, you will write a stored procedure that receives the school id and a leaders score as input parameters, calculates the icon setting and updates the fields appropriately.
- **Question 1:** Write the structure of a query to create or replace a stored procedure called UPDATE_LEADERS_SCORE that takes a in_School_ID parameter as an integer and a in_Leader_Score parameter as an integer. Don't forget to use the #SET TERMINATOR statement to use the @ for the CREATE statement terminator.
<br><br>
The screenshot for this question can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%204.JPG)</u>**

- **Question 2:** Inside your stored procedure, write a SQL statement to update the Leaders_Score field in the CHICAGO_PUBLIC_SCHOOLS table for the school identified by in_School_ID to the value in the in_Leader_Score parameter.

- **Question 3:** Inside your stored procedure, write a SQL IF statement to update the Leaders_Icon field in the CHICAGO_PUBLIC_SCHOOLS table for the school identified by in_School_ID using the following information.

**Score lower limit**| **Score upper limit** | **Icon**
---|:---|---
80|99|Very strong
60|79|Strong
40|59|Average
20|39|Weak
0|19|Very weak

**NOTE:** The following screenshot that answers Questions 2 and 3 can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%205%20and%206.JPG)</u>**


- **Question 4:** Run your code to create the stored procedure.
  - Write a query to call the stored procedure, passing a valid school ID and a leader score of 50, to check that the procedure works as expected.
<br><br>
The screenshot for this question can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Question%207.JPG)</u>**

#### Exercise 4: Using Transactions
You realize that if someone calls your code with a score outside of the allowed range (0-99), then the score will be updated with the invalid data and the icon will remain at its previous value. There are various ways to avoid this problem, one of which is using a transaction.
- **Question 1:** Update your stored procedure definition. Add a generic ELSE clause to the IF statement that rolls back the current work if the score did not fit any of the preceding categories.

- **Question 2:** Update your stored procedure definition again. Add a statement to commit the current unit of work at the end of the procedure.
 - Run your code to replace the stored procedure.
 - Write and run one query to check that the updated stored procedure works as expected when you use a valid score of 38.
 - Write and run another query to check that the updated stored procedure works as expected when you use an invalid score of 101.

**NOTE:** The screenshot for the above questions using transactions can be found **<u>[here](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/Week%206%20Project%20Assessment%20-%20HONORS/HONORS%20SQL%20Questions%208%20and%209.JPG)</u>**

### Resources
 - [SQL Basics Cheat Sheet](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/SQL%20Basics%20Cheat%20Sheet.jpg)
 - [SQL Cheat Sheet - Views, Stored Procedures, Transactions](https://github.com/collinbashore/IBM-Data-Science-Fundamentals-with-Python-and-SQL-Specialization/blob/main/04%20-%20Accessing%20SQL%20Databases%20using%20Python/SQL%20Cheat%20Sheet%20-%20Views%2C%20Stored%20procedures%2C%20Transactions%2C%20and%20JOIN%20Statements.jpg)

This course can also be found in multiple IBM programs. Completion of this course can be counted towards any of the following Specializations or Professional Certification programs:
- [IBM Data Science Professional Certificate](https://www.coursera.org/specializations/ibm-data-science)
- [Data Engineering Foundations Specialization](https://www.coursera.org/specializations/data-engineering-foundations)
- [Data Science Fundamentals with Python and SQL Specialization](https://www.coursera.org/specializations/data-science-fundamentals-python-sql)
- [IBM Data Analyst Professional Certificate](https://www.coursera.org/specializations/ibm-data-analyst)
- [Introduction to Data Science Specialization](https://www.coursera.org/specializations/introduction-data-science)
- [BI Foundations with SQL, ETL, and Data Warehousing Specialization](https://www.coursera.org/specializations/bi-foundations-sql-etl-data-warehouse)
- [IBM Data Engineering Professional Certificate](https://www.coursera.org/specializations/ibm-data-engineer)
- [IBM Data Warehouse Engineer Professional Certificate](https://www.coursera.org/specializations/data-warehouse-engineering)

Click on the link provided to access this course on Coursera: [Databases and SQL for Data Science with Python](https://www.coursera.org/learn/sql-data-science?specialization=data-science-fundamentals-python-sql)
