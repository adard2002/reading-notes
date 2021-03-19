# Reading 10 Notes

[Home](README.md)
## The Call Stack defined on MDN
### What is a call stack?
This is to keep track of multiple function and keeps track of what functions are being called and which are currently being run.
- When a script calls a function, the interpreter adds it to the call stack then starts to carry out the function.
- Any functions that are called by the function are added to the call stack. this is also when it runs where the calls are reached.
- When the current function is finished it is taken off of the stack and is resumed where ever it left off last.
- If the stack takes up more space than expected it will result in a error "stack overflow"

## Understanding the JavaScript Call Stack
In asychronous JavaScript we have a callback function, an event loop, and a task queue
- callback function: happens when acted by the callstack during execurtion after the callback has been pushed to the stack by event loop

## JavaScript error messages
- Reference Errors: This is when you have no declared the variable yet.
- Syntax Errors: Misspelling errors
- Range Errors: manipulates an object with some kind of length and give it an invalid length and this kind of errors will show up.
- Type Errors: Unidentified names
- 
## JavaScript errors reference on MDN 
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors
link to a lot of different errors to look at
