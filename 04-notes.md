# Reading 04 Notes

[Home](README.md)

# Classes & Memory Management

## Classes
- Declaring an object of type MyClass:
`MyClass mc = new MyClass();`

### Declaring Classes
- [access modifier] - [class] - [idendifier]
`public class Customer`

### Creating Objects
`Customer object1 = new Customer();`
 
# Constructors https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/constructors 
```
public class Person
{
   private string last;
   private string first;

   public Person(string lastName, string firstName)
   {
      last = lastName;
      first = firstName;
   }

   // Remaining implementation of Person class.
}
```

# Properties
What does a property do?
Enables a class to show a public way of getting and setting values.

What does the value keyword do?
It's used to define the assigned value using either  the set or init accessor

# Stack and Heap
- You can run out of memory even if there isn't a virtual address space to reserve a physical space to commit. 

# C# in a Nutshell - Chapter 3 
### Classes
A class can be: internal, abstract, sealed, static, unsafe, or partial. 

### Fields
A field is a variable that is a member of a class or struct:
```
class Unicorn
{
    string name;
    public int Age = 100;
}
```
