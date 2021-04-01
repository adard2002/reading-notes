# Reading 11 Notes

[Home](README.md)

# ERDs

## Research on What a Database Schema is:
1. What is a Schema?
Refers to the organization of data like a blueprint of how the databases are made or created. They are then divided into database tables.

2. Why do we use them?
A Database Schema tells you how the entities in a database relate to eachother like tables and views. This helps when software is going to interact with the database.

3. What do they look like?
They kind of look like a tree of some sort. Like what we did a couple labs ago with the animals and the zoo. We chose a section of "Animal" and they branched out into a few different groups like "Mammal" and "Reptile" and those groups branched out into animals that are mammals and reptiles. They are used for organizing.

## Research on what the different types of Database Keys are:
1. What is a Primary Key?
This is a column or set of columns in a table and the values are unique to identify a row in the table. 
2. What is a Foreign Key?
Collection or fields in one table. 
3. What is a Composite Key?
Example: If the Primary key is Student you would have Composite keys of Name, City, Age, Interests, etc.
4. How are they different? When do you use 1 over the other?
A foreign key is what is inside of a primary key 

## What are Relationships in a relational database?
1. What is a 1:1 relationship?
Only one row in a table that may be linked with only 1 row in another table. They are not a property of the data, but a relationship itself.
2. What is a Many:Many relationship?
Multiple rows in a table that may be linked with multiple rows in another table. 
3. How about a 1:Many or a Many:1?
This is when a parent record in 1 table can have a reference to several child records in another table. Whereas a many-to-many relationship a child record can link back to multiple parent records. 