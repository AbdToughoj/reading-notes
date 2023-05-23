## Class09: Ten Thousand 4

### **What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method.**

In Python, built-in operations or functionalities can have their behavior defined using dunder (double underscore) methods. They enable us to alter the behavior of objects in our code and override their default behavior.

One commonly used dunder method is **init**, which is used to initialize an object when it is created. Here's a short example:

```
class Person:
    def __init__(self, name):
        self.name = name

person = Person("Alice")
print(person.name)  # Output: "Alice"
```

In this example, the **init** method is called automatically when a Person object is created, allowing us to set the name attribute for that object.

### **In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?**

The main ethical issue raised in the video was the unauthorized use of developers' work without giving them proper credit or compensation. This could have been avoided by obtaining the necessary permissions and licenses for the developers' work or by collaborating with them directly, ensuring fair compensation and recognition for their contributions.

### **Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.**

The Python statistics module provides a set of functions for performing various statistical operations on data. It includes functions for calculating measures such as mean, median, mode, variance, and standard deviation.

One example function from the statistics module is mean(), which calculates the arithmetic mean of a list of values. Here's a short example:

```
python
import statistics

data = [1, 2, 3, 4, 5]
mean_value = statistics.mean(data)
print(mean_value)  # Output: 3
```

In this example, the mean() function from the statistics module is used to calculate the mean of the data list, which is 3.
