# 🐍 Python

## ⚙️ Operator Precedence (Highest to Lowest)

1. `**` → Exponent  
2. `%` → Modulo  
3. `//` → Floor Division  
4. `/` → Division  
5. `*` → Multiplication  
6. `-` → Subtraction  
7. `+` → Addition  
8. `=` → Assignment  

🧠 **Note:** Use parentheses `()` to override default precedence.

---

## 📦 Common Data Types

1. `int` → Integer  
2. `float` → Floating P oint  
3. `str` → String  
4. `bool` → Boolean
5. `None` → It is used as a placeholder. Value-without-a-value type thing.

➡️ Data types are called mutable if their value can be changed, and immutable if their value cannot be changed.
Example:
- Values within a List can be changed
- Changing individual letters within a string cannot happen
➡️ Therefore, a List is a mutable data type, while a string is an immuatable data type
---

## 🆚  Comparison Operators

1. `==` → Equal to
2. `!=` → Not Equal to
3. `<` → Less Than
4. `>` → Greater Than
5. `<=` → Less than or Equal to
6. `>=` → Greater than or Equal to
➡️ These operators return a `bool` value, ie: `True` **or** `False`
***NOTE:*** Only `==` and `!=` work with all data types, the rest work only with numeric data types

---
## 💾 Augmented Operators

1. `+=` → `a += x` is equal to `a = a + x`
2. `-=` → `a -= x` is equal to `a = a - x`
3. `*=` → `a *= x` is equal to `a = a * x`
4. `/=` → `a /= x` is equal to `a = a / x`
5. `%=` → `a %= x` is equal to `a = a % x`

---

## 🔍 Boolean Operators

➡️ They are used to compare boolean values

1. `and` → Outputs `True` **or** `False` if both values are `True` **or** `False` simulataneously. Otherwise, False.
Example:
- `True and False` outputs `False`
- `True and True` outputs `True`
- `False and False` outputs `False`

2. `or` → Outputs `True` if either one of the two values are `True`. Otherwise, False.
Example:
- `True or False` outputs True
- `False or False` outputs False

3. `not` → Unlike `and` and `or`, `not` is a unary operator as opposed to binary. It outputs the opposite boolean value.
Example:
- `not True` outputs `False`
- `not False` outputs `True`
---

## 🧠 Operator Behavior Based on Data Type

1. `+` → **Addition** for `int` and `float`  
   → **Concatenation** for `str`  
2. `*` → **Multiplication** for `int` and `float`  
   → **Replication** for `str` (e.g. `"yo" * 3` → `"yoyoyo"`)

---

## 🧾 Rules for Variable Names

1. Must be a **single word** (no spaces)  
   - ❌ `var one`  
   - ✅ `varone`
2. Can contain **letters**, **numbers**, and **only** underscore `_` as a special character
3. **Cannot begin** with a number  
   - ❌ `1name`  
   - ✅ `name1`

4. They are **Case Sensitive**

---

## 🖨️  Built-in Functions

### `print()`:-
➡️ Prints statements within quotes within parantheses.
Example: `print("Hello World!")` ***and*** `print('Hello World!')`
**NOTE:** An empty `print()` will be blank, and is used to skip lines

### `input()`:-
➡️ Takes an input from the user when the program is running.
**NOTE:** `input()` always returns a `str` type

### `len()`:-
➡️ Gives the length of the string argument.
Example: `len("Hello")` gives output as `5`
**NOTE:** Only works with `str` arguments, will give TypeError with `int` or `float`.

### `str()`:-
➡️ Converts the given parameter argument into a string data type.
Example: `str(8)` will return `'8'`

### `int()`:-
➡️ Converts the given parameter argument into an integer data type.
Example: `int('8')` will return `8`

### `float()`:-
➡️ Converts the given parameter argument into a floating point data type.
Example: `float('8')` will return `8.0`

### `range()`:-
➡️ Syntax is: `range(start, stop, step)`
➡️ `start` is the starting value, `stop` is the stopping value, and `step` is the value gap to be iterated.
**NOTE:** `range()` always stops at one value prior to the actual `stop` value.
Example:
```python
print(range(0,10,2))

Output will be:
0
2
4
6
8
```

---

## ⚖️ Flow Control Statements

### `if`:-
➡️ The block of the `if` statement will be executed if the condition is `True`. The clause is skipped if the condition is `False`.
Example:
```python
if name == 'Audi':
    print("Audi R8")
```

### `else`:-
➡️ The `if` clause can be followed by an `else` statement, which executes another condition **if** the original condition is `False`.
Example:
```python
if name == 'Audi':
    print("Audi R8")
else:
    print("BMW")
```

### `elif`:-
➡️ It is the else if statement, which allows multiple other conditions to be used if the original condition is `False`.
Example:
```python
if name == 'Audi':
    print("Audi R8")
elif name == 'BMW':
    print("BMW 5 Series")
```

### `while`:-
➡️ The code within a `while` statement will execute for as long as the condition remains `True`. It is also called the `while` loop.
Example:
```python
a = 0
while a < 5:
    print("Hello World")
    a = a + 1
```

### `break`:-
➡️ The `break` statement can be used to exit out of a `while` loop provided with a specific condition.
Example:
```python
name = ""
while True:
    print("Please type your name!")
    name = input()
    if name == 'your name':
        break
print("Thanks")
```

### `continue`:-
➡️ This is used within a loop. When the loop reaches this condition, it again goes back to the start of the loop and re-evaulates the loop.
Example:
```python
while True:
    print("Who are you?")
    name = input()
    if name != 'Joe':
        continue
    print("Password Please:")
    password = input()
    if password == 'abcd':
        break
print("Access Granted!)
```

### `for`:-
➡️ Executes a loop for a given number of times entered by the user.
Example:
```python
for i in range(5):
    print("Hello!")
    i = i + 1
```

### `sys.exit()`:-
➡️ Technically a function, but it is used for Flow Control. It is used to exit a program given a specific condition.
Example:
```python
import sys
while True:
    print("Enter exit to exit the program")
    res = input()
    if res == 'exit':
        sys.exit()
    else:
        continue
```

---

# 📑 Importing Modules

## `import`:-
➡️ Using `import` keyword, we import modules like `random`, `sys`, `os`, `math`, etc.
Example:
```python
import random, sys, os, math
```

## `from`:-
➡️ This is an alternate way to import modules
Example:
```python
from random import *
from sys import *
from os import *
from math import *
```

---
# 🪄 User Defined Functions

## `def` statement with arguments:
➡️ We use the `def` statement to define a function and then use that.
Example:
```python
def hello(name)
    print("Hello " + name)
hello("World!")
hello("Heisenberg")

Output will be:
Hello World
Hello Heisenberg
```

## `return` statment:
➡️ Used to return a specific value within a function.
Example:
```python
def hello(name):
    if name == 'Heisenberg':
        return "You're goddamn right"
    else:
        return 'Say my Name'
```
## Local and Global Scopes:
➡️ Parameters/Variables assigned **within** a function are **Local** parameters/variables.
➡️ Parameters/Variables assigned **outside** a function are **Global** parameters/variables.
**NOTE:**
1. Local Scope(s) from one function **cannot** use Local Scope(s) from another function.
2. Global Scope(s) **can** be read from Local Scope(s)
3. Different Local and Global variables ***can*** have the same name, but its a pain for us to read and understand.

### `global` statement:
➡️ Python allows to modify a global variable from within a function, this is how to do it.
Example:
```python
def spam():
    global eggs
    eggs = 'spam'
eggs = 'global'
spam()
print(eggs)

Output will be:
spam
```
---

# ⚠️ Exception Handling
➡️ We use `try` and `except` blocks to mitigate this.
Example:
```python
def spam(divideby):
    return 42/divideby
print(spam(42))
print(spam(0))

Output will be:
1.0
It will give ZeroDivisionError
```
➡️ Instead of getting an error, we use `try` and `except` to mitigate them.
Example:
```python
def spam(divideby):
    try:
        return 42/divideby
    except ZeroDivisionError:
        print("Error. Divide by Zero is forbidden")
print(spam(42))
print(spam(0))

Output will be:
1.0
Error. Divide by Zero is forbidden
```

---

# 📃 List and Tuple Data Types

## List
➡️ Its a value that contains multiple values within itself.
Example:
`l1 = [1,2,3]`
`l2 = ['A','B','C']`
➡️ The first value inside a list is on index zero (0).
➡️ The index value `-1` refers to the last value of the list.
Example:
```python
l = ['A','B','C']
print(l[0])
print(l[-1])

Output will be:
'A'
'C'
```
➡️ Full Syntax to slice a list: `list_name[start:stop:step]`
**NOTE:** Unlike the `range()`, this ***includes*** the `stop` index
➡️ The `len()` with a list gives the number of elements within that list.

### Changing Values within a List:
Example:
```python
l = [1,2,3,4]
print(l)
l[0] = 10
l[3] = 40
print(l)

Output will be:
[1,2,3,4]
[10,2,3,40]
```

### `+` and `*` operators with Lists:
➡️ `+` is used to concatenate Lists
➡️ `*` is used to replicate Lists
Example:
```python
l = [1,2,3]
m = [4,5,6]
print(l+m)
print(l*3)

Output will be:
[1,2,3,4,5,6]
[1,2,3,1,2,3,1,2,3]
```

### Deleting Statements within a List:

1. `del` Statement:
➡️ It takes an index argument and deletes the value at the specified index.
Example:
```python
l = [1,2,3,4]
del l[2]
print(l)

Output will be:
[1,2,4]
```

### `in` and `not in` Operators:
➡️ Gives a boolean value if the specified element is in the list or not.
Example:
```python
l = ['Hi', 'Hello', 'Bye']
print('Hi' in l)
print('Buh Bye' in l)

Output will be:
True
False
```

### Assigning Multiple Values at once:
For Example:
```python
l = [1,2,3]
l[0] = 10
l[1] = 20
l[2] = 30
```
➡️ We can do the following instead:
```python
l = [1,2,3]
10,20,30 = l
```
**NOTE:** The number of variables ***must*** be equal to the length of the string.

### List Methods:
➡️ A method is a function, but it differs from a function in a way that it is **called on** a value.

1. `index()`:
➡️ It will return the index position of the specified value argument.
Example:
```python
l = [1,2,3]
print(l.index(2))

Output will be:
1
```

2. `append()`:
➡️ It adds the specified argument value to the end of the list.
Example:
```python
l = [1,2,3]
l.append(4)
print(l)

Output will be:
[1,2,3,4]
```

3. `insert()`:
➡️ It inserts a value argument with an index argument. It's syntax: `insert(index, value)`
Example:
```python
l = [2,3,4]
l.insert(0,1)
print(l)

Output wil be:
[1,2,3,4]
```

4. `remove()`:
➡️ It removes the value argument from the list.
Example:
```python
l = [1,2,3,9,4]
l.remove(9)
print(l)

Output will be:
[1,2,3,4]
```
**NOTE:** If the value appears multiple times within the list, only the first one will be deleted.

5. `sort()`:
➡️ It is used to sort a list based on user's choice. By default, it sorts in ascending order, but can be revered using the `reverse = True` clause.
Example:
```python
l =  [1,4,3,2,6]
l.sort()
print(l)
l.sort(reverse = True)
print(l)

Output will be:
[1,2,3,4,6]
[6,4,3,2,1]
```
**NOTE:** This will not work if there are multiple data types within the list, aka, it will only work on homogeneous lists.
**Also NOTE:** The sort method on strings is in order of ASCII Values, so it prefers Capital letters first, then small, etc. To reverse it, use the `key = str.lower` clause.

## Tuple:
➡️ They're almost identical to Lists, but they use parantheses `()` and are **immutable**.
Example:
`t = (1,'A',2.3)` is a Tuple
**NOTE:** If your tuple needs only one value inside, it has to be followed by a comma, or else there will be a syntax error.
Example:
`t = ('N')` ❌
`t = ('N',)` ✅

## Interconversion using `list()` and `tuple()`:

### `list()`:
➡️ Use to convert a Tuple into a List
Example:
```python
t = (1,2,3)
l = list.(t)
```

### `tuple()`:
➡️ Use to convert a List into a Tuple
Example:
```python
l = [1,2,3]
t = tuple(l)
```