# DAY - 14 

=> still learning about OOP 

## Class and Instance Attributes in Python

=> Class attributes: Class attributes belong to the class itself they will be shared by all the instances. Such attributes are defined in the class body parts usually at the top, for legibility.

```python 
class sampleclass:
    count = 0     # class attribute

    def increase(self):
        sampleclass.count += 1

# Calling increase() on an object
s1 = sampleclass()
s1.increase()        
print(s1.count)

# Calling increase on one more
# object
s2 = sampleclass()
s2.increase()
print(s2.count)

print(sampleclass.count)
```
>1<br>
>2<br>
>2

#### Instance Attributes

=> Unlike class attributes, instance attributes are not shared by objects. Every object has its own 
copy of the instance attribute (In case of class attributes all object refer to single copy). To 
list the attributes of an instance/object, we have two functions:- 
1. vars() - This function displays the attribute of an instance in the form of an dictionary. 
2. dir() - This function displays more attributes than vars function,as it is not limited to instance. It displays the class attributes as well. It also displays the attributes of its ancestor classes.

```python 
# instance attributes.
class emp:
    def __init__(self):
        self.name = 'xyz'
        self.salary = 4000

    def show(self):
        print(self.name)
        print(self.salary)

e1 = emp()
print("Dictionary form :", vars(e1))
print(dir(e1))
```
>Dictionary form :{'salary': 4000, 'name': 'xyz'} <br>
>['__doc__', '__init__', '__module__', 'name', 'salary', 'show']

## Access Modifiers in Python 

=>Access modifiers in Python control which parts of a class can be accessed from outside the class, from within the class, or by subclasses. They help keep data and methods safe and organized.

### Types of Access Modifiers in Python

1.  Public Access Modifier
    - Members (variables or methods) declared as public can be accessed from anywhere in the program.
    - By default, all members are public in Python.

2.  Protected Access Modifier 
    - A member is considered protected if its name starts with a single underscore (_).
    - Convention only: It suggests that the member should not be accessed outside the class except by subclasses.
    - Still, Python allows direct access if explicitly called.

3. Private Access Modifier 
    - A member is private if its name starts with double underscores (__).
    - Python does not enforce strict privacy — instead, it uses Name Mangling.
    - The interpreter renames __var → _ClassName__var internally.
