# DAY 9 

today should be 10 day of writing in this repo but because i skip a day , today is day -9 . Today i learned about 

## loops 

#### while loop
    => while loop is the loop which checks the condition and run the code in other words the code keeps on running again and again   until the condition isn't false 

```python 
i = 0 # setting the value to one 
while i<5:   # if  i is smaller then 5 the code runs until the i is less then 5 
    print('learn with blake ')  
    i = i + 1  #incrementing the value of i by 1 to end the loop 

    while true: # it is infinite loop beacause the condition is always true
        print('learn with break ') 

#multiple of 5 
i = 0 
while i <= 10 : 
print(5*i)
i += 1 


```


---

#### range() in python 
```python
r = range(5)
print(type(x)) # <class "range">

r = range(1,10)
l = list(r)
print(l) # [1,2,3,4,5,6,7,8,9,]

r = range(10,20,3) # range with 3 parameters x,y,z , x , x + z , x + 2z .... till it is smaller then y 
l = list(r)
print(l) 

r = range(20,10,-3) # range with 3 parameters x,y,z , x , x - z , x - 2z .... till it is greater then y 
l = list(r)
print(l) 
```

---

#### for loop 
 => For loop is iterate through a sequence like set , tuple , list ,string  and range . 

 ```python 

# it prints all the items in l 
l = [10,20,30,40]
for x in l:
    print(x) # it prints all the items in l 

# it prints the number which gives the reminder 0 

for x in range(20): # range(n) which means number till n-1
    if x%6 == 0 :
        print(x) 

#multipication table of 3 
for i in range(1,11):
    print(3*i)


# writing a code to print table of any number 
n = int(input("enter the number which table you want to print"))
m = int(input("enter the number upto which you want to print the table " ))

for i in range(1,m+1):
    print(n*i)