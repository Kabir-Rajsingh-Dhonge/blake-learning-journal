### day-5 


today is second day of learning python , i learned about its variable and data type .

to write boolean we should write it with T capital and F capital e.g True and False 
None is like null in java . it's type is 'Nonetype'. just says empty 

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
y = 6 
x,y = y,x 
print(x)
print(y)


L = [10,20,30] // when you use [] python creates a list 
print(type(L))

l = (10,20,30) // tuple is which can't be modified . This is immutable . it is  written in () 

s = {10,20,30} // set = () the collection of key. math set operation are really fast.

d = { 10:"gfg",20:"idw"}  // dictionary is key - value pair 


### Tuple

Tuple is similar to list. it is immutable and faster then list but in list can add,remove , delete items and in tuple bracket is optional 

t = (10,20,"geeks")
print(t[0])  // it prints 10 

When to we use tuple

if 
   we type t = (10) // this is not the tuple it is int to make it tuple we should add comma in the end e.g 
   t = (10,) 


=> when creating the list we don't want to change through out the project or software life cycle 
e.g weekdays = ("sunday","monday"......)

t = 10,20,30,40,10 
                  output
print(t[2])       //30
print(t[-1])       //10 
print(t[1:3])      //(20,30)
print(len(t))     // 5
print(t.count(10)) // 2
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

A set is an unordered collection of unique elements—duplicates are automatically removed.

### Creating Sets

```python
s = {10, 20, 30}           # Direct creation
s = set()      # Converting a list to set
s = set()                  # Empty set (not {} which creates an empty dictionary)

Modifying Sets
python
s.add(item)                # Add a single item
s.update([items])          # Add multiple items from another collection
s.discard(item)            # Remove item if present; no error if missing
s.remove(item)             # Remove item; raises KeyError if missing
s.pop()                    # Remove and return an arbitrary item
s.clear()                  # Remove all items (set becomes empty)
del s                      # Delete the entire set variable

Membership Testing
python
print(item in s)           # Returns True or False

Set Operations

Method	Operator	Description

s1.union(s2)	s1 | s2	All items from both sets
s1.intersection(s2)	s1 & s2	Items common to both
s1.difference(s2)	s1 - s2	Items in s1 but not in s2
s1.symmetric_difference(s2)	s1 ^ s2	Items in either but not both

Set Comparisons
Method	Operator	Description

s1.isdisjoint(s2)	—	True if no common elements
s1.issubset(s2)	s1 <= s2	True if all items of s1 are in s2
—	s1 < s2	True if s1 is a proper subset
s1.issuperset(s2)	s1 >= s2	True if s1 contains all items of s2
—	s1 > s2	True if s1 is a proper superset

Dictionary
A dictionary is a collection of key-value pairs.

Characteristics
Unordered (insertion order preserved since Python 3.7+)

Keys must be unique and immutable (strings, numbers, tuples)

Values can be duplicated and of any type

Uses hashing internally for fast O(1) average lookups

Creating Dictionaries
python
d = {"name": "Ali", "age": 20}   # Direct creation
d = dict(name="Ali", age=20)     # Using dict() constructor
d = {}                           # Empty dictionary
d = dict()                       # Also empty dictionary

Accessing and Modifying
python
d["key"]                   # Access value; raises KeyError if missing
d.get("key")               # Access value; returns None if missing
d.get("key", default)      # Returns default if key missing
d["key"] = value           # Add or update key-value pair
d.update({"k1": v1})       # Add/update multiple pairs

Removing Items
python
d.pop("key")               # Remove key and return its value
d.pop("key", default)      # Return default if key missing
d.popitem()                # Remove and return last inserted pair
del d["key"]               # Delete a specific key
d.clear()                  # Remove all items

Useful Methods

python
d.keys()                   # Returns all keys
d.values()                 # Returns all values
d.items()                  # Returns key-value pairs as tuples
len(d)                     # Number of key-value pairs
"key" in d                 # Check if key exists
d.copy()                   # Shallow copy of dictionary

Dictionary Comprehension
python
squares = {x: x**2 for x in range(5)}  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
text

***


