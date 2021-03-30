# Reading 08 Notes

[Home](README.md)

# Collections & Enums

## C# 7.0 in a Nutshell: Pg 118-124


## Collections
### What is a collection and why are they used?
- Collections are pretty much exactly what the word collection means. Collections are used to group objects; creating arrays of objects. Each of these objects have their own little collection. 
- Arrays are really useful for creating Collections. Collections also provide an easier more flexible way to work with multiple groups of objects.
- In an array the grouped objects are able to be changed and formed however is wanted, with collections you can retrieve the object by using it's key or keyword.
- A collection is a class
### Kinds of Collections
#### 1. System.Collections.Generic classes: This can be used when every item in the collections has the same data type.
| Class | Description |
|:------|:-----------:|
| Dictionary<TKey,TValue> | Represents collection of key/value pairs organized based on their key
| List<T> | Represents a list of objects that can be accessed by the index. Some methods are search, sort, and modify lists.
| Queue<T> | Represents first in and first out collection of objects also known as FIFO
| SortedList<TKey,TValue> | Represents a collections of key/value pairs sorted by their key names
| Stack<T> | Similar to the Queue<T> but is instead a Last In First Out also known as LIFO

#### 2. System.Collections.Concurrent classes:
Using this method the collections in the namespace are safe thread-safe operations for collecting items from multiple threads

#### 3. System.Collections classes: Do not store elements as specific as typed objects, rather as objects of type Object
| Class | Description |
|:-----:|:-----------:|
| ArrayList | Represents an array objects whose size is increased as required
| Hashtable | Represents a collection of key/value pairs organized by the hashcode of their key
| Queue | Represents (FIFO) collection of objects
| stack | Represents (LIFO) collection of objects

Original Charts can be found on this site: ![Collections](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections)

## Enums
### What is an Enumeration type?
- "An enumeration type (or enum type) is a value type defined by a set of named constants of the underlying integral numeric type." The enumeration type can be defined by using the keyword of *enum* and epecify the names of the *enum members*.
Example:
``` enum Season
{
    Spring,
    Summer,
    Autumn,
    Winter
}
```
As you can see in this example the enum members are Spring, Summer, Autumn, and Winter. While the Season is the enumeration type. The constant values of enum members are of type int; meaning that they start with zero and increase by one.