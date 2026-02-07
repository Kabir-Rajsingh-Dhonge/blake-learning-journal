# DAY - 12 

=> Today  i am learning about file handling . why do we need file handling is to store data in it .we can also store data in databases but for small project , schoolwork using file for storage is best way to go .

## modes in file

=> There are various modes in which we can open files.

1. read (r): This mode opens the file for reading only and gives an error if the file does not exist. This is the default mode if no mode is passed as a parameter.

2. write (w): This mode opens the file for writing only and creates a new file if the file does not exist.

3. append (a): This mode opens the file for appending only and creates a new file if the file does not exist.

4. create (x): This mode creates a file and gives an error if the file already exists.

5. text (t): Apart from these modes we also need to specify how the file must be handled. t mode is used to handle text files. t refers to the text mode. There is no difference between r and rt or w and wt since text mode is the default. The default mode is 'r' (open for reading text, synonym of 'rt' ).

6. binary (b): used to handle binary files (images, pdfs, etc).

#### writing in file

=> when we open file in write or append mode if the file doesn't exist then it will create one . but in read it will give errors.

```python 

f = open('myfile.txt', 'w')
f.write('Hello, world!')
```

--- 

### Reading from the file 

```python 

f = open('myfile.txt', 'r')
contents = f.read()
print(contents)
```

---

### Appending to the file 

```python 

f = open('myfile.txt', 'a')
f.write('Hello, world!')
```

---

### Closing the file 

=> It is important to close a file after you are done with it. This releases the resources used by the file and allows other programs to access it.

To close a file, you can use the close() method.

```python 

f = open('myfile.txt', 'r')
# ... do something with the file
f.close() 
```

---

### With statement 

=>Alternatively, you can use the with statement to automatically close the file after you are 
done with it.
```python
with open('myfile.txt', 'r') as f:
    # ... do something with the file
    ```
- learned from = CodeWithHarry