---
layout: post
title:  "Notes of Python Chaper7-8"
date:   2020-08-16 13:56:29 +0800
categories: Python notes
---

## 【Automate the Boring Stuff with Python Practical Programming for Total Beginners】 

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

