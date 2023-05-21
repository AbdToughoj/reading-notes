## Class08: Ten Thousand 3

### What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.

```
new_list = [expression for item in iterable if condition]
```

In a list comprehension, the expression is evaluated for each item in the iterable, and the resulting value is added to the new list if the condition (if any) is met.

Using a for loop to create a list for squaring the elements in a given list of integers would look like this:

```
original_list = [1, 2, 3, 4, 5]
new_list = []
for num in original_list:
    new_list.append(num ** 2)
```

Using list comprehension, the same result can be achieved in a more concise manner:

```
original_list = [1, 2, 3, 4, 5]
new_list = [num ** 2 for num in original_list]
```

In this example, num \*\* 2 is the expression that squares each element num in original_list. The resulting squared values are automatically added to the new_list using list comprehension.

### What is a decorator in Python?

In Python, a decorator is a design pattern that allows the modification or extension of the behavior of a function, method, or class without directly modifying its code. It involves wrapping the original object with a higher-order function, providing additional functionality before, after, or around the original object's execution.

In Python, decorators provide a way to modify the behavior of functions or classes without directly modifying their source code. Decorators work by wrapping the original object with another function or class, enabling additional functionality.

### Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.

Common use cases for decorators include:

1. Adding functionality: Decorators can add extra behavior, such as logging, caching, or input validation, to functions or methods.
2. Modifying behavior: Decorators can alter the behavior of functions or methods by modifying their inputs, outputs, or execution flow.
3. Code organization: Decorators can be used to separate cross-cutting concerns, making code more modular and readable.

Here's an example of a simple decorator function:

```
python
def uppercase_decorator(func):
    def wrapper():
        original_result = func()
        modified_result = original_result.upper()
        return modified_result
    return wrapper

@uppercase_decorator
def greet():
    return "hello"

print(greet())  # Output: "HELLO"
```

In this example, the uppercase_decorator function is a decorator that wraps the greet function. It modifies the result of greet by converting it to uppercase before returning it. The @uppercase_decorator syntax is used to apply the decorator to the greet function. When greet() is called, it executes the modified behavior provided by the decorator.
