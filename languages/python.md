# Python

* Python is an interpreted, high-level, general-purpose, and dynamically typed programming language.
* It is also Object-oriented, supports modules and packages, and can be used as a scripting language.
* In Python, everything is an Object.
* Python files have an extension of `.py`.
* Python uses indentation to define code blocks instead of curly braces (`{}`).
* To run a Python file, use the following command in your terminal (Command Prompt on Windows, or shell on macOS/Linux):

    `$ python filename.py` or `$ python3 filename.py`

#### Python typically doesn't require explicit import statements for built-in functionalities.

## Creating and Executing a Program

1.  Open a terminal or command prompt.
2.  Create a Python file (e.g., `my_program.py`) using a text editor:
    *   On Linux/macOS: `nano my_program.py` or `vim my_program.py`
    *   You can also use any graphical text editor.
3.  Write your Python code in the file and save it.
4.  Execute the program from the terminal: `python my_program.py`

<br>

### Basic Datatypes

| Data Type | Description                                       | Example                       |
| :-------- | :------------------------------------------------ | :---------------------------- |
| `int`     | Integer values (whole numbers)                    | `0`, `1`, `-2`, `1000`        |
| `float`   | Floating-point values (numbers with decimals)     | `0.1`, `3.14`, `-2.5e-3`      |
| `str`     | Strings (sequences of characters)                 | `"hello"`, `'Python'`, `"""multi-line"""` |
| `bool`    | Boolean values (representing truth or falsehood)  | `True`, `False`               |
| `complex` | Complex numbers (numbers with a real and imaginary part) | `2+3j`, `1-4j`                |
| `NoneType`| Represents the absence of a value                 | `None`                        |

**Note:** Python does not have a separate `char` type. Single characters are represented as strings of length 1.

<br>

## Keywords

Keywords are reserved words in Python that have special meanings and cannot be used as variable names, function names, or any other identifiers. As of Python 3.10, there are 35 keywords.

| Keyword    | Description                                                    | Category                |
| :--------- | :------------------------------------------------------------- | :---------------------- |
| `True`     | Boolean value representing truth.                              | Value Keyword           |
| `False`    | Boolean value representing falsehood.                            | Value Keyword           |
| `None`     | Represents no value or a null value.                           | Value Keyword           |
| `and`      | Logical AND: returns `True` if both operands are true.         | Operator Keyword        |
| `or`       | Logical OR: returns `True` if either operand is true.          | Operator Keyword        |
| `not`      | Logical NOT: returns the opposite Boolean value.               | Operator Keyword        |
| `in`       | Membership test: returns `True` if a value is present in a sequence. | Operator Keyword        |
| `is`       | Identity test: returns `True` if two variables point to the same object. | Operator Keyword        |
| `if`       | Starts a conditional statement.                                | Conditional             |
| `elif`     | Else if: part of a conditional statement for multiple checks.  | Conditional             |
| `else`     | Part of a conditional statement; executes if the condition is false. | Conditional             |
| `for`      | Used for iterating over a sequence (e.g., list, tuple, string). | Iteration               |
| `while`    | Used for creating a loop that continues as long as a condition is true. | Iteration               |
| `break`    | Exits the current loop prematurely.                            | Iteration Control       |
| `continue` | Skips the rest of the code inside a loop for the current iteration and proceeds to the next. | Iteration Control       |
| `def`      | Defines a user-defined function.                               | Structure / Definition  |
| `class`    | Defines a user-defined class.                                  | Structure / Definition  |
| `lambda`   | Creates an anonymous (unnamed) function.                       | Structure / Definition  |
| `with`     | Used for resource management (e.g., file handling) to ensure resources are properly released. | Structure / Context     |
| `as`       | Used to create an alias, often with `import` or `with`.        | Structure / Alias       |
| `pass`     | A null operation; does nothing. Used as a placeholder.         | Structure               |
| `return`   | Exits a function and optionally returns a value.               | Returning Keyword       |
| `yield`    | Pauses a generator function and returns a value, preserving its state for the next call. | Returning Keyword       |
| `import`   | Imports modules or specific names from modules.                | Import                  |
| `from`     | Used with `import` to import specific parts of a module.       | Import                  |
| `try`      | Starts a block of code that might raise an exception.          | Exception Handling      |
| `except`   | Catches and handles exceptions raised in the `try` block.      | Exception Handling      |
| `finally`  | Defines a block of code that will be executed regardless of whether an exception occurred. | Exception Handling      |
| `raise`    | Manually raises an exception.                                  | Exception Handling      |
| `assert`   | Used for debugging; raises an `AssertionError` if a condition is false. | Exception Handling      |
| `async`    | Defines an asynchronous function (coroutine).                  | Asynchronous Programming |
| `await`    | Pauses execution of an `async` function until an awaitable object (e.g., another coroutine) completes. | Asynchronous Programming |
| `del`      | Deletes an object or a part of an object (e.g., an item from a list, a variable). | Variable Handling       |
| `global`   | Declares that a variable inside a function is global (defined outside the function). | Variable Handling       |
| `nonlocal` | Declares that a variable inside a nested function refers to a variable in an enclosing (non-global) scope. | Variable Handling       |

<br>

## Operators

| Operator Category      | Operator | Description                                                                 | Example                 |
| :--------------------- | :------- | :-------------------------------------------------------------------------- | :---------------------- |
| **Arithmetic**       | `+`      | Addition                                                                    | `x + y`                 |
|                        | `-`      | Subtraction                                                                 | `x - y`                 |
|                        | `*`      | Multiplication                                                              | `x * y`                 |
|                        | `/`      | Division (results in a float)                                               | `x / y`                 |
|                        | `//`     | Floor Division (discards the fractional part)                               | `x // y`                |
|                        | `%`      | Modulus (remainder of the division)                                         | `x % y`                 |
|                        | `**`     | Exponentiation (x raised to the power of y)                                 | `x ** y`                |
| **Comparison**       | `==`     | Equal to                                                                    | `x == y`                |
|                        | `!=`     | Not equal to                                                                | `x != y`                |
|                        | `>`      | Greater than                                                                | `x > y`                 |
|                        | `<`      | Less than                                                                   | `x < y`                 |
|                        | `>=`     | Greater than or equal to                                                    | `x >= y`                |
|                        | `<=`     | Less than or equal to                                                       | `x <= y`                |
| **Logical**          | `and`    | Logical AND: `True` if both operands are true                               | `x > 5 and y < 10`      |
|                        | `or`     | Logical OR: `True` if at least one operand is true                          | `x > 5 or y < 10`       |
|                        | `not`    | Logical NOT: `True` if the operand is false, `False` if the operand is true | `not (x == y)`          |
| **Bitwise**          | `&`      | Bitwise AND                                                                 | `x & y`                 |
|                        | `\|`     | Bitwise OR                                                                  | `x \| y`                |
|                        | `^`      | Bitwise XOR (Exclusive OR)                                                  | `x ^ y`                 |
|                        | `~`      | Bitwise NOT (Inverts all bits)                                              | `~x`                    |
|                        | `<<`     | Bitwise Left Shift                                                          | `x << 2`                |
|                        | `>>`     | Bitwise Right Shift                                                         | `x >> 2`                |
| **Assignment**       | `=`      | Assign value from right side to left side                                   | `x = 5`                 |
|                        | `+=`     | Add AND: `x = x + y`                                                        | `x += y`                |
|                        | `-=`     | Subtract AND: `x = x - y`                                                   | `x -= y`                |
|                        | `*=`     | Multiply AND: `x = x * y`                                                   | `x *= y`                |
|                        | `/=`     | Divide AND: `x = x / y`                                                     | `x /= y`                |
|                        | `//=`    | Floor Divide AND: `x = x // y`                                              | `x //= y`               |
|                        | `%=`     | Modulus AND: `x = x % y`                                                    | `x %= y`                |
|                        | `**=`    | Exponent AND: `x = x ** y`                                                  | `x **= y`               |
|                        | `&=`     | Bitwise AND assignment                                                      | `x &= y`                |
|                        | `\|=`    | Bitwise OR assignment                                                       | `x \|= y`               |
|                        | `^=`     | Bitwise XOR assignment                                                      | `x ^= y`                |
|                        | `>>=`    | Bitwise Right Shift assignment                                              | `x >>= y`               |
|                        | `<<=`    | Bitwise Left Shift assignment                                               | `x <<= y`               |
| **Identity**         | `is`     | Returns `True` if both variables are the same object                          | `x is y`                |
|                        | `is not` | Returns `True` if both variables are not the same object                    | `x is not y`            |
| **Membership**       | `in`     | Returns `True` if a sequence with the specified value is present in the object | `'H' in 'Hello'`        |
|                        | `not in` | Returns `True` if a sequence with the specified value is not present in the object | `'W' not in 'Hello'`    |
| **Parentheses**      | `( )`    | Grouping expressions, function calls, tuple declaration                     | `(a + b) * c`           |
| **List/Dict Access** | `[ ]`    | List indexing/slicing, dictionary key access, declaring lists             | `my_list[0]`, `my_dict['key']` |

<br>

## String Formatting (f-strings)

f-strings (formatted string literals) provide a concise and convenient way to embed expressions inside string literals for formatting. They were introduced in Python 3.6.

```python
name = "Alice"
age = 30
print(f"Hello, my name is {name} and I am {age} years old.")
# Output: Hello, my name is Alice and I am 30 years old.

pi = 3.14159
print(f"Pi to two decimal places: {pi:.2f}")
# Output: Pi to two decimal places: 3.14
```

<br>

## Basic Data Structures

### List

-   Lists are ordered, mutable (changeable) collections that allow duplicate members.
-   Created using square brackets `[]` or the `list()` constructor.

```python
# Creating lists
fruits = ["apple", "banana", "cherry"]
numbers = [1, 2, 3, 4, 5]
mixed_list = ["hello", 3.14, True, None]
empty_list = []
another_list = list(("apple", "banana")) # Using the constructor

# Accessing elements (indexing starts at 0)
print(fruits[0])  # Output: apple
print(fruits[-1]) # Output: cherry (last item)

# Slicing
print(fruits[1:3]) # Output: ['banana', 'cherry'] (items from index 1 up to, but not including, index 3)
print(fruits[:2])  # Output: ['apple', 'banana'] (from the beginning up to index 2)
print(fruits[1:])  # Output: ['banana', 'cherry'] (from index 1 to the end)

# Modifying lists
fruits[1] = "blueberry"
print(fruits) # Output: ['apple', 'blueberry', 'cherry']

# Adding elements
fruits.append("orange")   # Adds to the end
print(fruits) # Output: ['apple', 'blueberry', 'cherry', 'orange']
fruits.insert(1, "mango") # Inserts "mango" at index 1
print(fruits) # Output: ['apple', 'mango', 'blueberry', 'cherry', 'orange']

# Removing elements
fruits.remove("cherry") # Removes the first occurrence of "cherry"
print(fruits) # Output: ['apple', 'mango', 'blueberry', 'orange']
popped_fruit = fruits.pop() # Removes and returns the last element
print(popped_fruit) # Output: orange
print(fruits)       # Output: ['apple', 'mango', 'blueberry']
del fruits[0]       # Deletes the element at index 0
print(fruits)       # Output: ['mango', 'blueberry']

# Other common methods
print(len(fruits)) # Output: 2
if "mango" in fruits:
    print("Mango is in the list")
fruits.sort() # Sorts the list in place
print(fruits) # Output: ['blueberry', 'mango'] (alphabetical)
numbers.reverse() # Reverses the list in place
print(numbers)    # Output: [5, 4, 3, 2, 1]
```

-   `pop()` function removes the last item by default, or an item at a specified index.

    ```python
    thislist = ["apple", "banana", "cherry"]
    last_item = thislist.pop()
    print(last_item)         # Output: cherry
    first_item = thislist.pop(0)
    print(first_item)        # Output: apple
    print(thislist)          # Output: ['banana']
    ```

### Tuple

-   Tuples are ordered, immutable (unchangeable) collections that allow duplicate members.
-   Created using parentheses `()` or the `tuple()` constructor.

```python
# Creating tuples
point = (10, 20)
colors = ("red", "green", "blue", "red")
single_item_tuple = ("hello",) # Note the trailing comma
empty_tuple = ()
another_tuple = tuple(["a", "b", "c"]) # From a list

# Accessing elements (same as lists)
print(point[0])   # Output: 10
print(colors[1:3]) # Output: ('green', 'blue')

# Tuples are immutable - these operations will raise errors:
# point[0] = 5
# colors.append("yellow")

# Common operations
print(len(colors)) # Output: 4
print(colors.count("red")) # Output: 2 (counts occurrences)
print(colors.index("green")) # Output: 1 (returns index of first occurrence)

# Unpacking tuples
x, y = point
print(f"x: {x}, y: {y}") # Output: x: 10, y: 20
```
-   To create a tuple with only one item, you **must** add a comma after the item, otherwise Python will not recognize it as a tuple.
    ```python
    thistuple = ("apple",)
    print(type(thistuple)) # Output: <class 'tuple'>

    # NOT a tuple, this is just a string in parentheses
    not_a_tuple = ("apple")
    print(type(not_a_tuple)) # Output: <class 'str'>
    ```

### Set

-   Sets are unordered, mutable collections that do **not** allow duplicate members.
-   Created using curly braces `{}` (but not for an empty set, use `set()`) or the `set()` constructor.
-   Items are not indexed.

```python
# Creating sets
fruits = {"apple", "banana", "cherry", "apple"} # "apple" will only appear once
print(fruits) # Output might be {'cherry', 'banana', 'apple'} - order is not guaranteed

numbers = {1, 2, 3, 4, 5}
empty_set = set() # Important: {} creates an empty dictionary
another_set = set(["a", "b", "c"]) # From a list

# Adding elements
fruits.add("orange")
print(fruits)
fruits.update(["mango", "grape"]) # Adds multiple elements
print(fruits)

# Removing elements
fruits.remove("banana") # Raises KeyError if "banana" is not present
print(fruits)
fruits.discard("kiwi") # Does NOT raise an error if "kiwi" is not present
print(fruits)
popped_item = fruits.pop() # Removes and returns an arbitrary element
print(popped_item)
print(fruits)

# Set operations
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1.union(set2))          # Output: {1, 2, 3, 4, 5}  (or set1 | set2)
print(set1.intersection(set2))   # Output: {3}             (or set1 & set2)
print(set1.difference(set2))     # Output: {1, 2}          (or set1 - set2)
print(set1.symmetric_difference(set2)) # Output: {1, 2, 4, 5} (or set1 ^ set2)

print(len(fruits))
```

-   `frozenset()` is an immutable version of a set. Elements cannot be modified after creation.
    ```python
    set1 = {"apple", "banana", "cherry"}
    frzset = frozenset(set1)
    print(frzset)
    # frzset.add("orange") # This would raise an AttributeError
    ```

### Dictionary

-   Dictionaries are unordered (prior to Python 3.7, ordered since Python 3.7), mutable collections of key-value pairs.
-   Keys must be unique and immutable (e.g., strings, numbers, tuples).
-   Created using curly braces `{}` with `key: value` pairs or the `dict()` constructor.

```python
# Creating dictionaries
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}
empty_dict = {}
another_dict = dict(name="Bob", age=25) # Using the constructor

# Accessing values
print(person["name"]) # Output: Alice
print(person.get("age")) # Output: 30
print(person.get("country")) # Output: None (safer than [], doesn't raise KeyError)
print(person.get("country", "USA")) # Output: USA (provides a default value)

# Modifying dictionaries
person["age"] = 31 # Update existing value
person["occupation"] = "Engineer" # Add new key-value pair
print(person)

# Removing items
popped_value = person.pop("city") # Removes "city" and returns its value
print(popped_value) # Output: New York
print(person)
# del person["age"] # Deletes the key "age"
# print(person)

# Common methods
print(len(person)) # Output: 3 (number of key-value pairs)
print(list(person.keys()))   # Output: ['name', 'age', 'occupation'] (or similar, order depends on Python version)
print(list(person.values())) # Output: ['Alice', 31, 'Engineer']
print(list(person.items()))  # Output: [('name', 'Alice'), ('age', 31), ('occupation', 'Engineer')]

# Iterating
for key in person:
    print(f"{key}: {person[key]}")

for key, value in person.items():
    print(f"{key} -> {value}")
```

-   `pop()` function is used to remove an item with a specified key and return its value.
    ```python
    car = {
      "brand": "Ford",
      "model": "Mustang",
      "year": 1964
    }
    model = car.pop("model")
    print(model) # Output: Mustang
    print(car)   # Output: {'brand': 'Ford', 'year': 1964}
    ```

<br>

## Virtual Environments (`venv`)

It's highly recommended to use virtual environments for Python projects to manage dependencies and isolate project-specific package versions. Python's built-in `venv` module can be used for this.

1.  **Create a virtual environment:**
    Navigate to your project directory in the terminal and run:
    ```bash
    python3 -m venv myenv  # Replace 'myenv' with your desired environment name (e.g., venv, .venv)
    ```

2.  **Activate the virtual environment:**
    *   On macOS and Linux:
        ```bash
        source myenv/bin/activate
        ```
    *   On Windows (Command Prompt):
        ```bash
        myenv\Scripts\activate.bat
        ```
    *   On Windows (PowerShell):
        ```bash
        myenv\Scripts\Activate.ps1
        ```
    Your terminal prompt should change to indicate the active environment (e.g., `(myenv) $`).

3.  **Install packages:**
    With the environment active, use `pip` to install packages. They will be installed only in this environment.
    ```bash
    pip install requests
    pip freeze > requirements.txt # Save installed packages to a file
    ```

4.  **Deactivate the virtual environment:**
    When you're done working in the environment, you can deactivate it:
    ```bash
    deactivate
    ```

5.  **Recreating an environment from `requirements.txt`:**
    If you have a `requirements.txt` file, you can install all listed packages into an active virtual environment:
    ```bash
    pip install -r requirements.txt
    ```

<br>

## Conditional Branching (`if`, `elif`, `else`)

```python
x = 10
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")

# Single line if (less common for complex logic)
message = "Positive" if x > 0 else "Non-positive"
print(message)
```

<br>

## Loops

Python has two primary loop commands: `while` loops and `for` loops.

### `while` loop
-   Executes a set of statements as long as a condition is true.
```python
count = 0
while count < 5:
    print(f"Count is: {count}")
    count += 1
else: # Optional: executes when the loop condition becomes false
    print("Loop finished")
```
-   `break`: Exits the loop immediately.
-   `continue`: Skips the current iteration and proceeds to the next.

### `for` loop
-   Iterates over a sequence (list, tuple, dictionary, set, string) or other iterable objects.
```python
# Looping through a list
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

# Looping through a string
for char in "Python":
    print(char)

# Using range()
for i in range(5): # 0, 1, 2, 3, 4
    print(i)

for i in range(2, 5): # 2, 3, 4 (start, stop)
    print(i)

for i in range(0, 10, 2): # 0, 2, 4, 6, 8 (start, stop, step)
    print(i)
else: # Optional: executes after the loop finishes normally (not by break)
    print("For loop completed")

# Looping through dictionary keys
my_dict = {"a": 1, "b": 2}
for key in my_dict:
    print(f"Key: {key}, Value: {my_dict[key]}")

# Looping through dictionary items (key-value pairs)
for key, value in my_dict.items():
    print(f"Key: {key}, Value: {value}")
```
-   `pass`: If you have a loop or conditional block with no content, use `pass` to avoid an error.
    ```python
    for x in [0, 1, 2]:
        pass # Avoids an IndentationError
    ```

<br>

## Function Definition and Call

```python
# Defining a function
def greet(name):
    """This function greets the person passed in as a parameter.""" # Docstring
    message = f"Hello, {name}!"
    return message

def add(a, b=0): # b has a default value
    """This function adds two numbers."""
    return a + b

# Calling functions
greeting = greet("World")
print(greeting) # Output: Hello, World!

sum1 = add(5, 3)
print(sum1) # Output: 8

sum2 = add(7) # Uses default value for b
print(sum2) # Output: 7
```

*   You don't need to specify the return type of a function.
*   If a function doesn't have a `return` statement, or has a `return` statement without an expression, it implicitly returns `None`.
*   Functions can return any data type.
