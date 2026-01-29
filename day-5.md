### day-5 


today is second day of learning pyhon , i learned about its variable and data type .

to write boolean we should write it with T capital and F capital e.g True and Flase 
None is like null in java . it's type is 'Nonetpye'. just says empty 

replacing value in python 

a = 5 
b = 6 
temp = a 
a = b 
b = temp 
print(a)
print(b)

second way to replace

x = 5 
b = 6 
x,y = y,x 
print(x)
print(y)


L = [10,20,30]. // when you use [] python creates a list 
print(type(L))

l = (10,20,30) // tuble is which can't be modified . This is a List which is immutable . it is  written in () 

s = {10,20,30} // set = () the collection of key. math set operation are really fast.

d = { 10:"gfg",20:"idw"}  // distionary is key - value pair 


### Tubles 

Tables is similar to list. it is immutable and faster then list but in list can add,remove , delete items and in tables baracket is optional 

t = (10,20,"geeks")
print(t[0])  // it prints 10 

When to we use tables 

=> when creating the list we don't want to change through out the project or software life cycle 
e.g weekdays = ("sunday","monday"......)

t = 10,20,30,40,10 
                  output
print(t[2])       //30
print(t[-1])       //10 
print(t[1:3])      //(20,30)
print(len(t)).     // 5
print(t,count(10)) // 2
print(t.index(20))  // 1

## set

Python set is an unordered collection of multiple items having different datatypes. In Python, sets are mutable, unindexed and do not contain duplicates. The order of elements in a set is not preserved and can change.

Can store None values.
Implemented using hash tables internally.
Do not implement interfaces like Serializable or Cloneable.
Python sets are not inherently thread-safe; synchronization is needed if used across threads.
Creating a Set in Python

In Python, the most basic and efficient method for creating a set is using curly braces.

Python Sets can be created by using the built-in set() function with an iterable object or a sequence by placing the sequence inside curly braces, separated by a 'comma'.

Note: A Python set cannot contain mutable types such as lists or dictionaries, because they are unhashable.

