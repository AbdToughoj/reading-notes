## Class 03

### 1)What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

#### In Python, the with statement is used to open and handle files in a more secure and productive manner. Even if an error happens while the block of code is being performed, it makes sure that the file is properly closed thereafter. Through the prevention of resource leaks and potential problems that would arise if the file was not correctly closed, this aids in resource management while reading and writing files. The file object's close() method is automatically called when the with block is ended, so you don't need to explicitly call it when using the with statement. This strengthens your code, reduces the likelihood of errors, and can help you avoid future problems with resource management.

</br>

### 2)Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

#### To read data from a file object, use the read() and readline() functions. While the readline() function just reads one line from the file and returns it as a string, the read() method returns the full contents of the file as a single string. If you need to read a file's full contents as a single string, use read(); if you need to process the contents of a file one line at a time, use readline().

read() example:

```
with open('example.txt', 'r') as f:
    content = f.read()   # read the entire file
    print(content)
```

#### readline() example:

```
with open('example.txt', 'r') as f:
    line1 = f.readline()   # read the first line of the file
    line2 = f.readline()   # read the second line of the file
    print(line1)
    print(line2)
```

### 3)Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example

#### Detecting and dealing with problems that happen while a program is being run is known as exception handling. The try, except, and finally blocks in Python are used to manage exceptions and guarantee that code is executed correctly. The code that might cause an exception is contained in the try block, the code that is executed if an exception is raised is contained in the except block, and the code that is always executed, regardless of whether an exception is raised or not is contained in the finally block. These blocks enable you to gracefully manage exceptions, stop your program from crashing, and respond appropriately to exceptions.

#### Example:

```
try:
    x = int(input("Enter a number: "))
    y = 10 / x
    print("The result is", y)
except ValueError:
    print("Invalid input. Please enter a number.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
finally:
    print("Program execution complete.")
```
