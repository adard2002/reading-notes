# Reading 31 Notes

[Home](README.md)

# Razor Pages

## What are Razor Pages
Razor Pages application is technically MVC application and have the same features as MVC views. Razor Pages is a simplified web application programming model. The Razor Pages files are found under the Pages directory.

## Why Razor Pages?
1. Easier to get to web development for beginners because Razor Pages are not as in depth as MVC. There are people who come from other scripting languages like ASP or PHP who prefer Razor Pages than MVC
2. Razor Pages fit better to smaller scenarios where building controllers and models as separate classes are overkill.

The Razor Pages can make coding page-focused scenarios easier than using controllers and views. 

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
