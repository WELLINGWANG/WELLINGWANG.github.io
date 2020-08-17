---
layout: post
title:  "Notes For Python Chaper1-3"
date:   2020-08-15 09:56:29 +0800
categories: Python notes
---

## 【Automate the Boring Stuff with Python Practical Programming for Total Beginners】 

## **Chapter 1**. **Python Basics** 

#### Covers expressions, the most basic type of Python instruction, and how to use the Python interactive shell software to experiment with code.

   ![image001](F:\mindi abair\notes for AUTOMATE.files\image001.png)                            

**The Integer, Floating-Point, and String Data Types**

 ![image002](F:\mindi abair\notes for AUTOMATE.files\image002.png)

**String Concatenation and Replication**

**Storing Values in Variables**

 **Assignment Statements**

 **Variable Names**

 \1. It can be only one word.

 \2. It can use only letters, numbers, and the underscore (_) character.

 \3. It can’t begin with a number.

 \4. It is a Python convention to start your variables with a lowercase letter.

 ![image003](F:\mindi abair\notes for AUTOMATE.files\image003.png)

**Dissecting Your Program**

**Comments**

**The print() Function**

 When writing a function name, the opening and closing parentheses at the end identify it

 as the name of a function. This is why in this book you’ll see print() rather than print.

**The input() Function**

**The len() Function**

**The str(), int(), and float() Functions**

It is good to remember the different types of operators (+, -, *, /, //, %, and ** for math

operations, and + and * for string operations) and the three data types (integers, floatingpoint

numbers, and strings) introduced in this chapter.



### **Chapter 2**. **Flow Control**  

#### Explains how to make programs decide which instructions to execute so your code can intelligently respond to different conditions.

**Boolean Values**

 the Boolean values True and False lack the quotes you place around strings, and they always start with a capital *T* or *F*

**Comparison Operators**

*Comparison operators* compare two values and evaluate down to a single Boolean value.

(**THE DIFFERENCE BETWEEN THE == AND = OPERATORS)**

![image004](F:\mindi abair\notes for AUTOMATE.files\image004.png)                               

**Boolean Operators**

three Boolean operators (and, or, and not)

**Binary Boolean Operators**

**The not Operator**

**Mixing Boolean and Comparison Operators**

\>>> **2 + 2 == 4 and not 2 + 2 == 5 and 2 \* 2 == 2 + 2**

True

**Elements of Flow Control**

Flow control statements start with conditions, and all are followed by

a block of code called the *clause*.

**Conditions**

**Blocks of Code**

\1. Blocks begin when the indentation increases.

\2. Blocks can contain other blocks.

\3. Blocks end when the indentation decreases to zero or to a containing block’s indentation.

**Program Execution(f5)**

**Flow Control Statements**

**if Statements**

 ![image005](F:\mindi abair\notes for AUTOMATE.files\image005.png)

**else Statements**

An if clause can optionally be followed by an else statement.

**elif Statements**

 ![image006](F:\mindi abair\notes for AUTOMATE.files\image006.png)

**while Loop Statements**

***\*break Statements**

There is a shortcut to getting the program execution to break out of a while loop’s clause early. If the execution reaches a break statement, it immediately exits the while loop’s clause. In code, a break statement simply contains the break keyword.

(An infinite loop that *never* exits is a common programming bug.)

***\*continue Statements**

continue statements are used inside loops. When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop and reevaluates the loop’s condition. (This is also what happens when the execution reaches the end of the loop.)

**(Ctrl+C to terminate program immediately.)**

**You can use** **continue** **and** **break** **statements only inside** **while** **and** **for** **loops.** 

![image007](F:\mindi abair\notes for AUTOMATE.files\image007.png) 

 ![image008](F:\mindi abair\notes for AUTOMATE.files\image008.png)

**for Loops and the range() Function**

 ![image009](F:\mindi abair\notes for AUTOMATE.files\image009.png)

**The Starting, Stopping, and Stepping Arguments to range()**

The range() function is flexible in the sequence of numbers it produces for for loops. *For* example (I never apologize for my puns), you can even use a negative number for the step argument to make the for loop count down instead of up.

for i in range(5, -1, -1):

  print(i)

Running a for loop to print i with range(5, -1, -1) should print from five down to

  zero.

**Importing Modules**

 ![image010](F:\mindi abair\notes for AUTOMATE.files\image010.png)

 ![image011](F:\mindi abair\notes for AUTOMATE.files\image011.png)

**from import Statements**

 ![image012](F:\mindi abair\notes for AUTOMATE.files\image012.png)

**Ending a Program Early with sys.exit()**

The last flow control concept to cover is how to terminate the program. This always happens if the program execution reaches the bottom of the instructions. However, you can cause the program to terminate, or exit, by calling the sys.exit() function. Since this function is in the sys module, you have to import sys before your program can use it. Open a new file editor window and enter the following code, saving it as *exitExample.py*:

![image013](F:\mindi abair\notes for AUTOMATE.files\image013.png) 

**

### **Chapter 3**. **Functions**

####  Instructs you on how to define your own functions so that you can organize your code into more manageable chunks.

A *function* is like a mini-program within a program.

**defines a function named ; the body of the function; function calls.**

A major purpose of functions is to group code that gets executed multiple times.

![image014](F:\mindi abair\notes for AUTOMATE.files\image014.png) 

 ![image015](F:\mindi abair\notes for AUTOMATE.files\image015.png)

**def Statements with Parameters**

➊. A *parameter* is a variable that an argument is stored in when a function is called. ➋. One special thing to note about parameters is that the value stored in a parameter is forgotten when the function returns. This is similar to how a program’s variables are forgotten when the program terminates.

**Return Values and return Statements**

 ![image016](F:\mindi abair\notes for AUTOMATE.files\image016.png)

Remember, expressions are composed of values and operators. A function call can be used in an expression because it evaluates to its return value.

**The None Value**

In Python there is a value called None, which represents the absence of a value.

 ![image017](F:\mindi abair\notes for AUTOMATE.files\image017.png)

**Keyword Arguments and print()**

***\*end=''**

 ![image018](F:\mindi abair\notes for AUTOMATE.files\image018.png)

***\*sept=','**

![image019](F:\mindi abair\notes for AUTOMATE.files\image019.png) 

**Local and Global Scope**

Parameters and variables that are assigned in a called function are said to exist in that function’s *local scope*. Variables that are assigned outside all functions are said to exist in the *global scope*. A variable that exists in a local scope is called a *local variable*, while a variable that exists in the global scope is called a *global variable*. A variable must be one or the other; it cannot be both local and global.

A local scope is created whenever a function is called.

![image020](F:\mindi abair\notes for AUTOMATE.files\image020.png) 

The reason Python has different scopes instead of just making everything a global variable is so that when variables are modified by the code in a particular call to a function, the function interacts with the rest of the program only through its parameters and the return value.

While using global variables in small programs is fine, it is a bad habit to rely on global variables as your programs get larger and larger.

**Local Variables Cannot Be Used in the Global Scope**

**Local Scopes Cannot Use Variables in Other Local Scopes**

A new local scope is created whenever a function is called, including when a function is called from another function. Consider this program.

Multiple local scopes can exist at the same time.

The upshot is that local variables in one function are completely separate from the local variables in another function.

**Global Variables Can Be Read from a Local Scope**

 ![image021](F:\mindi abair\notes for AUTOMATE.files\image021.png)

**Local and Global Variables with the Same Name**

**The global Statement**

 ![image022](F:\mindi abair\notes for AUTOMATE.files\image022.png)

There are four rules to tell whether a variable is in a local scope or global scope:

\1. If a variable is being used in the global scope (that is, outside of all functions), then it is always a global variable.

\2. If there is a global statement for that variable in a function, it is a global variable.

\3. Otherwise, if the variable is used in an assignment statement in the function, it is a local variable.

\4. But if the variable is not used in an assignment statement, it is a global variable.

![image023](F:\mindi abair\notes for AUTOMATE.files\image023.png) 

 ![image024](F:\mindi abair\notes for AUTOMATE.files\image024.png)

This error happens because Python sees that there is an assignment statement for eggs in the spam() function ➊ and therefore considers eggs to be local. But because print(eggs) is executed before eggs is assigned anything, the local variable eggs doesn’t exist. Python will *not* fall back to using the global eggs variable ➋.

**FUNCTIONS AS “BLACK BOXES”**

**Exception Handling**

Errors can be handled with try and except statements. 

 ![image025](F:\mindi abair\notes for AUTOMATE.files\image025.png)

![image026](F:\mindi abair\notes for AUTOMATE.files\image026.png)

 

 