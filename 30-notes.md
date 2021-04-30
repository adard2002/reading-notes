# Reading 30 Notes

[Home](README.md)

# Implementation: Hash Tables

## What is a Hashtable?
### Terminology:
1. Hash: This is what happpens as a result of some algorithm taking an input of a string and converting it into a value that can be used for security or another purpose. In this case (a hashtable) it's used to tell what the index of an array is. A hash is the ability to encode the key that will eventually map to a specific location in the data structure which we can look at directly and retrieve the value
2. Buckets: This is what is contained in each index of the array of the hashtable. Every index is a bucket and the index can contain mulitple keys or value pairs if a collision occurs.
3. Collisions: This is what it is called when more than one key gets hashed into the same location of the hashtable.

### Why are Hashtables used?
1. Hold unique Values
2. Dictionary
3. Library

### What are they?
Hashtables are a datastructure that use key value pairs. Every *Node* or *Bucket* has both a key and a value. Hashtables are usually used for storing the key into the data structure and being able to quickly retrieve the value. This is called a hash. A Hash code turns a key into an integer. *Hash codes should never have randomness to them. And that same key should always produce the same hash code.* 

### Creating a hash
1. Add or multiply all the ASCII values together
--- What is an ASCII value? American Standard Code for Information Interchange. This means a character encoding standard for electronic communication.
2. Multiply it by a prime number like 599
3. Use modulo to get the remainder of the result when divided by the total size of the array.
4. Insert in the array at that specific index.

#### Example:
```
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 
```