# Reading 14 Notes

[Home](README.md)
# DATABASE NORMALIZATION
## Database Normalization Explained in Simple English
### What is database normalization 
Organizes databases into rows and columns making them into a table. This contains very specific tasks along with specific topics. 
Limiting each table to just one process will help with possible duplication of a certain topic. 
### Why would you use database normalization?
There are 3 main reasons we do this:
1. Minimize duplicate data
2. Minimize data modification issues
3. Simplify queries
### Data duplication and modification anomalies
Why is duplicated information not good to have? 
1. Increases uneeded storage and decreases the performance
2. Becomes more difficult to manage data changes
### Definition of Database Normalization
There are 3 common forms of database normalization: 1st, 2nd, and 3rd normal form. Also can be abbreviated as 1NF, 2NF, and 3NF. These forms are progressive, meaning that you need to satisfy the rules for 2nd normal form in order to qualify for the 3rd. And you need the 1st normal form in order to qualify for the 2nd. Here is a summary of the various forms:
1. First Normal Form - This info is stored in a relational table with each column containing atomic values. Meaning there are no repeating groups of columns.
2. Second Normal Form - The table is in the first normal form. All of the columns depend on the tables primary key.
3. Third Normal Form - This table is in the second normal form and it's columns are not transitively dependent on the primary key.
