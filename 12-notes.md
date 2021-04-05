# Reading 12 Notes

[Home](README.md)

# Entity Framework Core and APIs

## Entity Framework Core
Entity Framework Core is a cross-platform version of the data access technology. Some benefits of this can be:
1. Enabling .NET developers to work with a database using .NET objects.
2. Gets rid of the need for most data-access code that is usually written. 

### The Model
With the EF Core, the data access is performed using a model. A model is made up of entity classes and objects that represent a session with the database. This is used to query and save data. EF supports these model development approaches:

- Generating a model from an existing database
- Hand code a model matching the database
- Once a model is created, EF Migrations can be used to create a database from the model. Migrations allow building off of the database as the model changes.

## Data Seeding
### What is data seeding?
This is the process of populating a database with an initial set of data.



