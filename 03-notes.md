# Reading 03 Notes

[Home](README.md)

# File Manipulation / System.I.O

## File and Stream I/O
What is a namespace?
These go toward the beginning of your c# file and contain types that enable reading and writing both synchronously and asynchronously on data streams and files. 

Streams is an abstract base class. Streams involve 3 operations:
1. Reading - transferring data from a stream into a data structure
2. Writing - Transfterring data from a data source into a stream
3. Seeking - querying and modifying the current position within a stream.

## Write to a file
Classes and methods typically used for writing text to a file: 
- StreamWriter: contains methods to write to a file synchronously
- File: provides static methods to write text to a file
- Path: used for strings that have file or directory path information

## Read to a file
the System.IOs are usually used for writing and reading data rather than character strings. 