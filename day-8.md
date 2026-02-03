# DAY - 8 


today i learn about if , else ,elif in python , elif is something new i am going to use . as i have been using if else in c .


## i made a simple calculator using if,else,elif function .

    ```python

 # making simple calculations with cpython

a = int(input('Enter the first number'))
b = int(input('Enter the second number'))

c = int(input('type 1 for sub.'
              ' \ntype 2 for sub \n'
              'type 3 for mul. \n'
              'dtype 4 for division'))

if c == 1 :
    d = a + b 
    print("the sum of two numbers is :", d)
elif c == 2:
    d = a - b 
    print('the subtraction of two numbers is :',d)
elif c == 3:
    d = a*b
    print('the multiple of two numbers is :', d)
elif c == 4:
    d= a/b
    print('the division of two numbers is :', d)
else:
    print(' the input is invalid') 
    
```
---
```python 

#printing the largest number 

a = int(input('enter the first number'))
b = int(input('enter the second number'))
c = int(input('enter the third number'))


if c<a and b<a:
    print(' largest number is ',a)
elif c < b : 
    print("largest number is ",b)
else :
    print('largest number is ',c) 

```
---
```python 

#finding if the year is leap year 

a = int(input('Enter a year'))

if a % 4 == 0 and (a % 100 != 0 or a % 400 == 0) :
   print('the year is leap year')
else :
    print("it isn't a leap year")
