# Reading 01 Notes

[Home](README.md)

## Exception Handling

### Debugging for absolute beginners
1. Clarify the problem and ask yourself: What did you expect your code to do? and What did it do instead?
2. Examine your assumptions: Before you begin to debug you should ask yourself if your using an API correctly, any simple typos such a missing semicolon or a space or missing curly brace. Anything simple as that, go through your code and double check you have everything that you want and maybe you are just missing a little line of code.
You can debug by going to the right of your editor right next to the number lines and click. What should show up is a little red dot which can be thought of as a stop sign. This will make the debugger run through your code until it hits that specified line where you put the dot. This is to find where exactly your code messed up.

### Try/Catch Blocks
1. Try Block:
- Place any code statements that might give an exception here
- If the code might throw any of multiple expressions place them in a try block

2. Catch Block:
- Place any statements used to handle the exception(s) in one or more catch blocks below the try block.
- Each catch block includes an exception type and is able to contain other statements needed to handle that exception type.
- Multiple catch blocks catch the exceptions and display the results to the console.
- The CLR catches exceptions not handles by catch blocks.

### Exception Handling
Statement keywords-
| Category | C# Keywords |
|:---------|:-----------:|
| Selection statements | if, else, switch, case |
| Iteration statements | do, for, foreach, in, while |
| Jump statements | break, continue, default, goto, return, yield |
| Exception handling statements | throw, try-catch, try-finally, try-catch-finally |
| Checked and unchecked | checked, unchecked |
| Fixed statement | fixed |
| Lock statement | lock |

## Therac-25
This was a computer-controlled radiation therapy. It had some major issues and was involved in at least six accidents between 1985 and 1987. The accidents were to do with the machine giving people radiation doses hundreds times greater than normal. This caused some serious injuries and even death. These accidents were because the software was designed so it was pretty much impossible to test in a clean automated way. It had to do a lot with the design of the software and there were even messages displayed "MALFUNCTION" which was follows from a number within the range of 1 to 64.

## Ariane 5
Ariane 5 is a European Space Agency or ESA. It's been used to deliver payloads into GTO or a transfer orbit. This rocket had a streak of 85 successful launches. It would return or go into orbit around the ocean area so if there was an error it could land in the ocean and not cause any problems.

With C# I find it weird how the curly braces are on their own lines. I keep wanting to put it next to the method and such where it would normally go in JS.