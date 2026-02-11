# DAY - 13 Fundamental of OOP 

=> So i learned about the oop in python today . This topic overwhelmed for the first time in this learning journey of python .   


## Four Pillars of OOP in Python

=> Overview of the four pillars of the OOP in python 

1. Inheritance
    - Inheritance allows a class (child class) to acquire properties and methods of another class (parent class). It supports hierarchical classification and promotes code reuse.

2. Polymorphism
    - Polymorphism in Python means "same operation, different behavior." It allows functions or methods with the same name to work differently depending on the type of object they are acting upon.
    The flowchart below represents the different types of polymorphism in Python, showing how a single interface can exhibit multiple behaviors at compile-time and run-time.

3. Encapsulation
    - Encapsulation is the bundling of data (attributes) and methods (functions) within a class, restricting access to some components to control interactions. A class is an example of encapsulation as it encapsulates all the data that is member functions, variables, etc.

4. Data Abstraction
    - Abstraction hides the internal implementation details while exposing only the necessary functionality. It helps focus on "what to do" rather than "how to do it."


## Class 

=>A class in Python is a user-defined template for creating objects. It bundles data and functions together, making it easier to manage and use them. When we create a new class, we define a new type of object. We can then create multiple instances of this object type.

> creating a class 

```python 

class human: # defining class
    haircolor = "black" #class attribute
```

## Object

=>An object is a specific instance of a class. It holds its own set of data (instance variables) and can invoke methods defined by its class. Multiple objects can be created from same class, each with its own unique attributes.

> creating a object 

```python 
class human:
    haircolor = "black"

human1 = human() # Creating object from class
print(human1.haircolor) # Accessing the class

```

##### OUTPUT

> black 

### Initiate Object with __init__()

=>The __init__() method acts as a constructor in Python and is automatically executed when an object is created. It is used to initialize the attributes of the object with the values provided at the time of object creation.

```python 
class human:
    haircolor = "black"

    def __init__(self, name, age):
        self.name = name  # Instance attribute
        self.age = age  # Instance attribute

# Creating an object of the human class
human1 = human("blake", 19)

print(human1.name)  
print(human1.haircolor)
```
##### OUTPUT 

>blake<br>
>black

### __str__() Method

=> __str__ method in Python allows us to define a custom string representation of an object. By default, when we print an object or convert it to a string using str(), Python uses the default implementation, which returns a string like <__main__.ClassName object at 0x00000123>.

```python 
class human:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __str__(self):
        return f"{self.name} is {self.age} years old."
human1 = human("Blake", 19)
human2 = human("Kabir", 21)

print(human1)  
print(human2)
```

##### OUTPUT
>Blake is 19 years old.<br>
>Kabir is 21 years old. 
