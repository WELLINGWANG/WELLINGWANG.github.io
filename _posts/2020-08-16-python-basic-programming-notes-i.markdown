---
layout: post
title:  "Notes For Python Chaper4-6"
date:   2020-08-15 09:56:29 +0800
categories: Python notes
---

## 【Automate the Boring Stuff with Python Practical Programming for Total Beginners】 

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

![image062](F:\mindi abair\notes for AUTOMATE.files\image061.png)

***The copy Module’s copy() and deepcopy() Functions**

![image062](F:\mindi abair\notes for AUTOMATE.files\image062.png) 

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

 