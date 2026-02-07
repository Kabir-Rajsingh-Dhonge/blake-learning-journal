# DAY - 11

I read about the function how the function are created and why do we need them . I learn about it yesterday .


## Function 

=> Function is the set of instruction which can be reused any number of time 

---

### Appilacation of the function 
1. Avoid code redundancy amd ease maintance
2. make code modular
    - takeinput()
    - processData()
    - processOutput()
3. Abstraction ( for example , in library function. we don't have to woeey about internal working )
4. Avoid variable name collisions 

---

### Syntax of function 

```python 

def fun():   # def function_name(parameter):
    print("fun() is called ")

print("before the function is called ")
fun()

#output 
""" before the function is called 
fun() is called """

```

---

```python

def getDate(d,m,y):
    return d + "-" + m + "-" + y 

print(" Blake was born on ")
date = getDate("30","01","2007")
print(date)

#output 
"""  
 Blake was born on 
30-01-2007 """
 ```

 ---

 #### keyword argument

=> The value can be send in two ways positional way and keyword way . The above program gives it by positonal way .

```python 

def print_details(id,name,address):
        print(f"id is {id}")
        print(f"name is {name}")
        print(f"address is {address}")

print_details(name = "blake", id="11",address="Nepal")
print()

""" output 
id is 11
name is blake
address is Nepal """
```

---

##### using position argument
```python

def print_details(id,name,address):
        print(f"id is {id}")
        print(f"name is {name}")
        print(f"address is {address}")

print_details("blake","11","Nepal")
print()

""" output 
id is blake
name is 11
address is Nepal """
```
As we can see if use position argumenr i input blake in first what it does is give blake to id which we should give to name . So with the help of keyword argument we can give parameter form any position but in positional argument must match the order of parameters in the function definition.

---

> *args allows a function to take any number of positional arguments, stored as a tuple
> **kwargs allows a function to take any number of keyword arguments, stored as a dictionary.




