
- There are two types of datatypes, Primitive, and Abstract,
	- There are 5 main primitive datatypes.
		- These are [[0- Data Types - Introduction#Int|Int]] , [[0- Data Types - Introduction#Float|Float]] , [[0- Data Types - Introduction#Bool|Bool]] , [[0- Data Types - Introduction#Char|Char]] , [[0- Data Types - Introduction#String|String]]


# Primitive Datatypes

### Int

Int, or Integers, are Whole numbers, such as 1, 42, and 23343


### Float

Float, or Floating Point, are Decimal numbers, such as 3.14, 1412.123, and 1.00


### Bool

Bool, or Boolean, is True or False
	Linked with Binary, which is just 1 or 0 [[1- Number Systems#Binary|Binary]]


### Char

Char, or Characters are a single item from a character set such as ASCII or UNICODE, 
e.g. "A", "g" or "4"
> Notice that there are "" around them, so even though a number is shown, it is a character due to its datatype, and we can tell from the quotations

### String

Strings are multiple Characters **"Stringed"** together, such as "Hello", "1234" and "44hlkklh)@"


--------------------------------


# Abstract Datatypes

- Abstract Datatypes are **User Defined Datatypes**, or in other words, are not provided to you by the language you are writing in (Those are called [[1- Arrays, Lists, Tuples, Records, Dictionaries|Primitve Data Structures]])
	- For example, if you are writing a [[2- Stacks|Stack]] in an **Object Oriented** fashion, then you might want to have each piece of data held inside of a "Node".
		- This "Node" is not an actual datatype, but by writing a class and giving it Initial values, you have essentially created your own Datatype.
		> See [[2- Stacks|Stacks]], [[3- Queues|Queues]], [[4- Linked Lists||Linked Lists]], [[5- Binary Trees||Binary Trees]], and  [[6- Graphs|Graphs]] to see how we can use Abstract Datatypes to form Abstract Data Structures.



-------------------------------------------------------

# Type Casting

- With our primitive Datatypes, some of them are quite similar, (e.g. Float and Int, and depending on the situation, string and int/float)
	- In some cases, we might not want our data in that specific type, so - If possible - we can **Cast** our data to a different type.
		- E.g. we could change the int 2412 into the string "2412", which we may want depending on the situation

Python Syntax
```
Num = 2413
Num = str(Num)
print(type(Num))

----------------------------------

Output: <class 'str'>
```