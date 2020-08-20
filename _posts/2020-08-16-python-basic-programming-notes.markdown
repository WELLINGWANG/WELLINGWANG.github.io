---
layout: post
title:  "Notes of Python loading..."
date:   2020-08-16 09:56:29 +0800
categories: Python notes
---

## 【Automate the Boring Stuff with Python Practical Programming for Total Beginners】 

### **Chapter 1**. **Python Basics** 

#### Covers expressions, the most basic type of Python instruction, and how to use the Python interactive shell software to experiment with code.

   ![image001](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image001.png)                            

**The Integer, Floating-Point, and String Data Types**

 ![image002](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image002.png)

**String Concatenation and Replication**

**Storing Values in Variables**

 **Assignment Statements**

 **Variable Names**

 \1. It can be only one word.

 \2. It can use only letters, numbers, and the underscore (_) character.

 \3. It can’t begin with a number.

 \4. It is a Python convention to start your variables with a lowercase letter.

 ![image003](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image003.png)

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

![image004](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image004.png)                               

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

 ![image005](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image005.png)

**else Statements**

An if clause can optionally be followed by an else statement.

**elif Statements**

 ![image006](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image006.png)

**while Loop Statements**

***\*break Statements**

There is a shortcut to getting the program execution to break out of a while loop’s clause early. If the execution reaches a break statement, it immediately exits the while loop’s clause. In code, a break statement simply contains the break keyword.

(An infinite loop that *never* exits is a common programming bug.)

***\*continue Statements**

continue statements are used inside loops. When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop and reevaluates the loop’s condition. (This is also what happens when the execution reaches the end of the loop.)

**(Ctrl+C to terminate program immediately.)**

**You can use** **continue** **and** **break** **statements only inside** **while** **and** **for** **loops.** 

![image007](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image007.png) 

 ![image008](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image008.png)

**for Loops and the range() Function**

 ![image009](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image009.png)

**The Starting, Stopping, and Stepping Arguments to range()**

The range() function is flexible in the sequence of numbers it produces for for loops. *For* example (I never apologize for my puns), you can even use a negative number for the step argument to make the for loop count down instead of up.

for i in range(5, -1, -1):

  print(i)

Running a for loop to print i with range(5, -1, -1) should print from five down to

  zero.

**Importing Modules**

 ![image010](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image010.png)

 ![image011](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image011.png)

**from import Statements**

 ![image012](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image012.png)

**Ending a Program Early with sys.exit()**

The last flow control concept to cover is how to terminate the program. This always happens if the program execution reaches the bottom of the instructions. However, you can cause the program to terminate, or exit, by calling the sys.exit() function. Since this function is in the sys module, you have to import sys before your program can use it. Open a new file editor window and enter the following code, saving it as *exitExample.py*:

![image013](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image013.png) 

**

### **Chapter 3**. **Functions**

####  Instructs you on how to define your own functions so that you can organize your code into more manageable chunks.

A *function* is like a mini-program within a program.

**defines a function named ; the body of the function; function calls.**

A major purpose of functions is to group code that gets executed multiple times.

![image014](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image014.png) 

 ![image015](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image015.png)

**def Statements with Parameters**

➊. A *parameter* is a variable that an argument is stored in when a function is called. ➋. One special thing to note about parameters is that the value stored in a parameter is forgotten when the function returns. This is similar to how a program’s variables are forgotten when the program terminates.

**Return Values and return Statements**

 ![image016](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image016.png)

Remember, expressions are composed of values and operators. A function call can be used in an expression because it evaluates to its return value.

**The None Value**

In Python there is a value called None, which represents the absence of a value.

 ![image017](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image017.png)

**Keyword Arguments and print()**

***\*end=''**

 ![image018](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image018.png)

***\*sept=','**

![image019](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image019.png) 

**Local and Global Scope**

Parameters and variables that are assigned in a called function are said to exist in that function’s *local scope*. Variables that are assigned outside all functions are said to exist in the *global scope*. A variable that exists in a local scope is called a *local variable*, while a variable that exists in the global scope is called a *global variable*. A variable must be one or the other; it cannot be both local and global.

A local scope is created whenever a function is called.

![image020](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image020.png) 

The reason Python has different scopes instead of just making everything a global variable is so that when variables are modified by the code in a particular call to a function, the function interacts with the rest of the program only through its parameters and the return value.

While using global variables in small programs is fine, it is a bad habit to rely on global variables as your programs get larger and larger.

**Local Variables Cannot Be Used in the Global Scope**

**Local Scopes Cannot Use Variables in Other Local Scopes**

A new local scope is created whenever a function is called, including when a function is called from another function. Consider this program.

Multiple local scopes can exist at the same time.

The upshot is that local variables in one function are completely separate from the local variables in another function.

**Global Variables Can Be Read from a Local Scope**

 ![image021](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image021.png)

**Local and Global Variables with the Same Name**

**The global Statement**

 ![image022](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image022.png)

There are four rules to tell whether a variable is in a local scope or global scope:

\1. If a variable is being used in the global scope (that is, outside of all functions), then it is always a global variable.

\2. If there is a global statement for that variable in a function, it is a global variable.

\3. Otherwise, if the variable is used in an assignment statement in the function, it is a local variable.

\4. But if the variable is not used in an assignment statement, it is a global variable.

![image023](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image023.png) 

 ![image024](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image024.png)

This error happens because Python sees that there is an assignment statement for eggs in the spam() function ➊ and therefore considers eggs to be local. But because print(eggs) is executed before eggs is assigned anything, the local variable eggs doesn’t exist. Python will *not* fall back to using the global eggs variable ➋.

**FUNCTIONS AS “BLACK BOXES”**

**Exception Handling**

Errors can be handled with try and except statements. 

 ![image025](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image025.png)

![image026](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image026.png)

 ![image027](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image027.png)

 ### **Chapter 4**. **Lists**

####  Introduces the list data type and explains how to organize data.

  ![image028](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image028.png))                             

**Getting Individual Values in a List with Indexes**

The integer inside the square brackets that follows the list is called an

*index*.

![image029](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image026.png)

 ![image030](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image030.png)

 ![image031](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image031.png)

**Negative Indexes**

The integer value -1 refers to the last index in a list.

**Getting Sublists with Slices**

Just as an index can get a single value from a list, a *slice* can get several values from a list, in the form of a new list.

 ![image032](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image032.png)

 ![image033](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image033.png)

**Getting a List’s Length with len()**

**Changing Values in a List with Indexes**

 ![image034](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image034.png)

**List Concatenation and List Replication**

 ![image035](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image035.png)

**Removing Values from Lists with del Statements**

 ![image036](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image036.png)

**Working with Lists**

 ![image037](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image037.png)

***Using for Loops with Lists**

 ![image038](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image038.png)

**The in and not in Operators**

**The Multiple Assignment Trick**

The number of variables and the length of the list must be exactly equal, or Python will give you a ValueError.

 ![image039](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image039.png)

**Augmented Assignment Operators**

![image040](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image040.png) 

The += operator can also do string and list concatenation:

 ![image041](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image041.png)

**Methods**

 ![image042](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image042.png)

**Finding a Value in a List with the index() Method**

 ![image043](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image043.png)

**Adding Values to Lists with the append() and insert() Methods**

Methods belong to a single data type. The append() and insert() methods are list methods and can be called only on list values, not on other values such as strings or integers.

 ![image044](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image044.png)

***\**Removing Values from Lists with remove()**

 ![image045](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image045.png)

**>>>spam.remove('bat')**  equals to  **del spam[1]**

 ![image046](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image046.png)

**Sorting the Values in a List with the sort() Method**

 ![image047](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image047.png)

![image048](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image048.png) 

![image049](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image049.png) 

 ![image050](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image050.png)

 ![image051](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image051.png)

**List-like Types: Strings and Tuples**

 ![image052](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image052.png)

**Mutable and Immutable Data Types**

**(The difference between overwriting and modifying.)**

 ![image053](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image053.png)

 ![image054](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image054.png)

**The Tuple Data Type**

tuples are typed with parentheses, ( and ), instead of square brackets, [ and ].

that tuples, like strings, are

immutable.

 ![image055](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image055.png)

 ![image056](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image056.png)

**Converting Types with the list() and tuple() Functions**

 ![image057](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image057.png)

***References**

 ![image058](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image058.png)

 ![image059](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image059.png)

 ![image060](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image060.png)

Variables will contain references to list values rather than list values themselves. But for strings and integer values, variables simply contain the string or integer value. Python uses references whenever variables must store values of mutable data types, such as lists or dictionaries. For values of immutable data types such as strings, integers, or tuples, Python

variables will store the value itself.

![image061](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image061.png)

***The copy Module’s copy() and deepcopy() Functions**

![image062](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image062.png) 

If the list you need to copy contains lists, then use the copy.deepcopy() function instead of copy.copy(). The deepcopy() function will copy these inner lists as well.

 

 

 

 

### **Chapter 5**. **Dictionaries and Structuring Data** 

#### Introduces the dictionary data type and shows you more powerful ways to organize data.

**Dictionaries vs. Lists**

Unlike lists, items in dictionaries are unordered.

Because dictionaries are not ordered, they can’t be sliced like lists.

 ![image063](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image063.png)

**The keys(), values(), and items() Methods**

 ![image064](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image064.png)

 ![image065](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image065.png)

 ![image066](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image066.png)

![image067](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image067.png) 

 ![image068](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image068.png)

**Checking Whether a Key or Value Exists in a Dictionary**

 ![image069](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image069.png)

**The get() Method**

 ![image070](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image070.png)

***\*The setdefault() Method**

 ![image071](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image071.png)

 ![image072](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image072.png)

 ![image073](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image073.png)

**Pretty Printing**

 ![image074](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image074.png)

 ![image075](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image075.png)

**Using Data Structures to Model Real-World Things**

**Nested Dictionaries and Lists**

 

### **Chapter 6**. **Manipulating Strings**

 Covers working with text data (called *strings* in Python).

**Working with Strings**

**Double Quotes**

 ![image076](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image076.png)

**Escape Characters**

 ![image077](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image077.png)

![image078](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image078.png) 

**Raw Strings**

![image079](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image079.png) 

**Multiline Strings with Triple Quotes**

string. Python’s indentation rules for blocks do not apply to lines inside a multiline string.

**Multiline Comments**

**Indexing and Slicing Strings**

**The in and not in Operators with Strings**

**Useful String Methods**

 ![image080](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image080.png)

**The isX String Methods**

 ![image081](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image081.png)

 ![image082](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image082.png)

**The startswith() and endswith() String Methods**

**The join() and split() String Methods**

 ![image076](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image083.png)

**Justifying Text with rjust(), ljust(), and center()**

![image084](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image084.png) 

  ![image085](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image085.png)

**Removing Whitespace with strip(), rstrip(), and lstrip()**

 ![image086](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image086.png)

 ![image087](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image087.png)

**Copying and Pasting Strings with the pyperclip Module**

**Project: Adding Bullets to Wiki Markup**

**Step 1: Copy and Paste from the Clipboard**

**Step 2: Separate the Lines of Text and Add the Star**

**Step 3: Join the Modified Lines**

 ![image088](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image088.png)

 ### **Chapter 7**. **Pattern Matching with Regular Expressions**

####  Covers how Python can manipulate strings and search for text patterns with regular expressions.

**Finding Patterns of Text Without Regular Expressions**

**Finding Patterns of Text with Regular Expressions**

**Creating Regex Objects**

 ![image089](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image089.png)                              

\>>> import re

\>>> phoneNumRegex = re.compile(r'\d\d\d-\d\d\d-\d\d\d\d')

Matching Regex Objects

 ![image090](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image090.png)

 ![image091](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image091.png)

***\*Review of Regular Expression Matching**

 ![image092](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image092.png)

**More Pattern Matching with Regular Expressions**

**Grouping with Parentheses**

Adding parentheses will create *groups* in the regex: (\d\d\d)-(\d\d\d-\d\d\d\d).

Passing 0 or nothing to the group() method will return the entire matched text.

 ![image093](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image093.png)

 ![image094](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image094.png)

 ![image095](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image095.png)

***Matching Multiple Groups with the Pipe**

 ![image096](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image096.png)

 ![image097](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image097.png)

**Optional Matching with the Question Mark**

 ![image098](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image098.png)

You can think of the ? as saying, “Match zero or one of the group preceding this question mark.”

If you need to match an actual question mark character, escape it with \?.

**Matching Zero or More with the Star**

The * (called the *star* or *asterisk*) means “match zero or more” — the group that precedes the star can occur any number of times in the text.

 ![image099](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image099.png)

If you need to match an actual star character, prefix the star in the regular expression with a backslash, \\*.

**Matching One or More with the Plus**

 ![image100](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image100.png)

If you need to match an actual plus sign character, prefix the plus sign with a backslash to escape it: \\+.

***Matching Specific Repetitions with Curly Brackets**

For example, the regex (Ha){3} will match the string 'HaHaHa', but it will not match 'HaHa', since the latter has only two repeats of the (Ha) group.

For example, (Ha){3,} will match three or more instances of the (Ha) group, while (Ha){,5} will match zero to five instances.

 ![image101](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image101.png)

**Greedy and Nongreedy Matching**

 ![image102](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image102.png)

 ![image103](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image103.png)

Note that the question mark can have two meanings in regular expressions: **declaring a nongreedy match** or **flagging an optional group**.

***The findall() Method**

findall() will not return a Match object but **a list of strings** — *as long*

*as there are no groups in the regular expression*.

 ![image104](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image104.png)

If there *are* groups in the regular expression, then findall() will return **a list of tuples**.

![image105](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image105.png) 

 ![image106](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image106.png)

***\**Character Classes**

 ![image107](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image107.png)

 ![image108](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image108.png)

![image109](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image109.png) 

 ![image110](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image110.png)

***Making Your Own Character Classes**

 ![image111](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image111.png)

 ![image112](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image112.png)

 ![image113](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image113.png)

Now, instead of matching every vowel, we’re matching every character that isn’t a vowel.

***The Caret and Dollar Sign Characters**

 ![image114](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image114.png)

![image115](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image115.png) 

**“Carrots cost dollars”

 ![image116](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image116.png)

***\*The Wildcard Character**

The . (or *dot*) character in a regular expression is called a *wildcard* and will match any character except for a newline.

 ![image117](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image117.png)

 ![image118](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image118.png)

**Matching Everything with Dot-Star**

 ![image119](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image119.png)

 ![image120](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image120.png)

 ![image121](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image121.png)

 ![image122](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image122.png)

**Matching Newlines with the Dot Character**

 ![image123](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image123.png)

***\**\*Review of Regex Symbols**

 ![image124](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image124.png)

**Case-Insensitive Matching**

![image125](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image125.png) 

**Substituting Strings with the sub() Method**

 ![image126](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image126.png)

 ![image127](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image127.png)

**Managing Complex Regexes**

This “verbose mode” can be enabled by passing the variable re.VERBOSE as the second argument to re.compile().

 ![image128](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image128.png)

***\**Combining re.IGNORECASE, re.DOTALL, and re.VERBOSE**

 ![image129](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image129.png)

 

**

### **Chapter 8**. **Reading and Writing Files** 

#### Explains how your programs can read the contents of text files and save information to files on your hard drive. How to use Python to create, read, and save files on the hard drive

**Files and File Paths**

**Backslash on Windows and Forward Slash on OS X and Linux**

On **Windows,** paths are written using **backslashes (*****\*****)** as the separator between folder names. **OS X and Linux,** however, use the **forward slash (*****/\*****)** as their path separator. If you want your programs to work on all operating systems, you will have to write your Python scripts to handle both cases.

 ![image130](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image130.png) 'usr\\bin\\spam'

\>>>import os

print(os.path.join('F:\\','mindi abair','works','ace'))

![image131](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image131.png) 

![image132](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image132.png) 

**The Current Working Directory**

 ![image133](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image133.png)

**Absolute vs. Relative Paths**

 ![image134](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image134.png)

 ![image135](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image135.png)

 ![image136](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image136.png)

***\**Creating New Folders with os.makedirs()**

 ![image137](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image137.png)

That is, os.makedirs() will create any necessary intermediate folders in order to ensure that the full path exists.

 ![image138](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image138.png)

***The os.path Module**

**Handling Absolute and Relative Paths**

 ![image139](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image139.png)

 ![image140](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image140.png)

 ![image141](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image141.png)

 ![image142](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image142.png)

 ![image143](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image143.png)

**Finding File Sizes and Folder Contents**

 ![image144](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image144.png)

 ![image145](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image145.png)

 ![image146](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image146.png)

**Checking Path Validity**

 ![image147](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image147.png)

 ![image148](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image148.png)

***\*****The File Reading/Writing Process**

***Plaintext files\*** contain only basic text characters and do not include font, size, or color information. Text files with the ***.txt\*** **extension** or Python

script files with the ***.py\*** **extension** are examples of plaintext files.

***Binary files\*** are all other file types, such as word processing documents, PDFs, images, spreadsheets, and executable programs.

 ![image149](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image149.png)

 ![image150](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image150.png)

**Opening Files with the open() Function**

 ![image151](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image151.png)

The call to open() returns a **File** **object**. A File object represents a file on your computer; it is simply **another type of value** in Python, much like the lists and dictionaries you’re already familiar with.

*******Reading the Contents of Files**

the contents of a file as a single large string value

 ![image152](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image152.png)

***readlines()\*** ***method\*** to get a *list* of string values from the file, one string for each line of text.

 ![image153](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image153.png)

**Writing to Files**

You can’t write to a file you’ve opened in read mode, though. Instead, you need to open it in “write plaintext” mode or “append plaintext” mode, or *write mode* and *append mode* for short.

import os

defeat=open('F:\\mindi abair\\works\\deff.txt','a') #open or create a new txt

defeat.write('Life is short.\nYou took it for granted, then it\'s gone.\n')

defeat.close()

 ![image154](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image154.png)

**Saving Variables with the shelve Module**

The **shelve** **module** will let you add Save and Open features to your program.

**###os.getcwd()###**

 ![image155](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image155.png)

Your programs can use the shelve module to later **reopen** and **retrieve** the data from these shelf files. *Shelf values don’t have to be opened in read or write mode — they can do both once opened.*

 ![image156](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image156.png)

Just like dictionaries, shelf values have **keys()** and **values()** methods that will return listlike values of the keys and values in the shelf.

 ![image157](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image157.png)

**Saving Variables with the pprint.pformat() Function**

pprint.pprint() function will “pretty print” the contents of a list or dictionary to the screen

pprint.pformat() function will return this same text as a string instead of printing it

 ![image158](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image158.png)

*And since Python scripts are themselves just text files with the *.py* file extension, **your Python programs can even generate other Python programs.**

 ![image159](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image159.png)

***Project: Generating Random Quiz Files**

Each time through the loop, the %s placeholder in 'capitalsquiz%s.txt' and

'capitalsquiz_answers%s.txt' will be replaced by (quizNum + 1)

**random.sample()** **function**

 ![image160](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image160.png)

 ![image161](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image161.png)

![image162](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image162.png) 

 ![image163](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image163.png)

**Project: Multiclipboard**

The ***.pyw\*** **extension** means that Python won’t show a Terminal window when it runs this program. (See Appendix B for more details.)

 ![image164](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image164.png)

 ![image165](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image165.png)

 ![image166](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/pythonotes/image166.png)



### Chapter 9. 

#### Organizing Files Shows how Python can copy, move, rename, and delete large numbers of files much faster than a human user can. It also explains compressing and decompressing files.

### Chapter 10.

####  Shows how to use Python’s various bug-finding and bug-fixing tools.

### Chapter 11. 

#### Shows how to write programs that can automatically download web pages and parse them for information. This is called web scraping.

### Chapter 12. 

#### Covers programmatically manipulating Excel spreadsheets so that you don’t have to read them. This is helpful when the number of documents you have to analyze is in the hundreds or thousands.

### Chapter 13. 

#### Covers programmatically reading Word and PDF documents.

### Chapter 14. 

#### Continues to explain how to programmatically manipulate documents with CSV and JSON files.

### Chapter 15. 

#### Explains how time and dates are handled by Python programs and how to schedule your computer to perform tasks at certain times. This chapter also shows how your Python programs can launch non-Python programs.

### Chapter 16.

####  Explains how to write programs that can send emails and text messages on your behalf.

### Chapter 17. 

#### Explains how to programmatically manipulate images such as JPEG or PNG files.

### Chapter 18.

####  Explains how to programmatically control the mouse and keyboard to automate clicks and keypresses.