# Reading 21 Notes

[Home](README.md)

# Roles, Claims and JWT Tokens

## Authentication with ASP.NET Core
### Difference between Authentication and Authorisation
These are both for security reasons which determines what a user can and cannot do and proves whether or not the user is really the user they are trying to sign into.
1. Authentication: This is the process of telling who you are. Proving that you are really you to avoid people who are trying to get into your account
2. Authorisation: This is the process of telling you what you can and cannot do. Like permissions like an administrator should be the only one to delete something from your account or whatever the role may be.

## Claims-based authentication
This can be thought of as a statement about or property of or a particular identity. This statement contains a name and a vlaue. As an example DateOfBirth tells about what the identity is not what it can do. 

## Claims-based authorization in ASP.NET Core
- A claim is a name value pair that tells what the subject is. Not what the subject can do. Claims based authorization checks the value of a claim allowing access for certain users based upon that value. 
