# DAY - 10 

today is fifth day of learning python and i have wrote some basic program and learn some basic topic of python i still have some basic topics to cover before i learn advance topic on it . 


### Break statement in python 
=> Break statement helps to come out of the loop immediately  

```python 
i = 1 
while i <= 5 : #if i is less then 5 loop continue 
    if i == 4: # if i is 4 
        break  #  then the loop will end 
    print(i) #printing the current value of  i 
    i = i + 1 #incrementing the value of i 
print(i) # after loop being end the value of i will be printed 
```

---

### Continue statement in Python
=> Continue statement skips and continue from the next steps.

```python 
l = [10,16,17,18,19,15] # list of numbers 
for i in l: # go through each item in list
    if i % 5 == 0: # if the is divisible by 5 
        continue.  #skip it and move to next item
    print(x).      #print the number which is not divisible by 5
```

---

### Nested loop 
=> Nested loop means loop inside the loop , it can be while loop inside for loop , for loop inside for loop , for loop inside while loop and so on . 

```python 
  for i in range(1,3): 
    j=1
    while j<3:
        print(i,j)
        j = j + 1
    print("blake")
```