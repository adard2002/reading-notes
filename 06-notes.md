# Reading 06 Notes

[Home](README.md)

# Object Oriented Principles

## Inheritance
Inheritance allows you to create classes which can reuse, extend, and change behaviors defined in other classes. 
Derived Class Example: If you have a base class (the members that are inherited) Animal, You might have a derived class (the one who inherits those members) Mammal or Reptile. Mammal and Reptile are both animals but are derived classes with different specifications. 

## Abstract Classes and Class Members
### Abstract Classes:
Provides a definition of the base class that multiple derived classes can share

## Polymorphism
Polymorphism means "many forms" and it is when we have many classes related to eachother or are inherited with eachother. Inheritance is when you take a class and kind of divide up into different groups. Like for example a class of Tarantula; Tarantula could be divided up into 2 groups or types of Tarantula; Arboreal and Terrestrial. Arboreal and Terrestrial would be Derived classes of Tarantula. Each derived class will have their own unique output or feature. 
Example of what the code would look like:
``` 
class Tarantula  // Base class (parent) 
{
  public void tarantulaType() 
  {
    Console.WriteLine("Tarantulas can be either Arboreal or Terrestrial");
  }
}

class Arboreal : Tarantula  // Derived class (child) 
{
  public void tarantulaType() 
  {
    Console.WriteLine("The arboreals are better at climbing");
  }
}

class Terrestrial : Tarantula  // Derived class (child) 
{
  public void tarantulaType() 
  {
    Console.WriteLine("The Terrestrials are not as good as climbing and tend to stay on the level ground");
  }
}
```

## OOP Principles
4 key techniques used in object-oriented programming (like c#) are:
1. Abstraction: Groups of related properties, methods, and other members are treated as one
2. Encapsulation: Hides unnecessary details from type consumers
3. Inheritance: Allows you to create a new class based on an existing class. Kind of like what was talked about above
4. Polymorphism: Can have multiple classes within one.




