# Reading 16 Notes

[Home](README.md)

# Data Transfer Objects

## Create Data Transfer Objects (DTOs)
### What is a DTO?
DTO is an object that defines how the data will be sent to the network. DTOs are usually used to return data back to the presentation layer. This is helpful for decoupling clients from your internal data structures.
Without DTO your API can only expose the database entities to the client and recieve data that maps directly to your database tables. This is not always a good idea. Using DTO will allow you do these:
- Remove circular references
- Hide particular properties that are not supposed to be viewed by clients.
- Omit some properties to reduce payload size

### Why would you use DTOs?
If you are using models to pass data between layers and sending data back to the presentation layer, you are exposing the internal details and data structures of your application. You would also want to use DTOs for data hiding.  

### Using DTOs for data hiding
This returns only data that is requested. 