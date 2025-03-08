<h1>
  <span class="headline">Intro to Python for Scripting</span>
  <span class="subhead">Input, Output, and </span>
</h1>

**Learning objective:** By the end of this lesson, students will understand how Python handles operators, and user input and output.

## User input and output

Python provides built-in functions to display output and interact with the user.

### Output

We've already seen that Python provides the `print()` function to display output. The `print()` function can take multiple arguments, which will be printed in the order you provide them. For example:

`intro_to_python.py`

```python
print("The sum of 2 and 3 is", 2 + 3)
```

In the first line, the `print()` function displays a message and the result of the expression `2 + 3`.

You can also use string formatting to create more complex output. For example, you can use f-strings to embed variables or expressions within a string:

`intro_to_python.py`

```python
name = "Alice"
age = 25
print(f"My name is {name}, and I am {age} years old.")
# Prints: "My name is Alice, and I am 25 years old."
```

### User input

You can use the `input()` function to get input from the user. It prompts the user to enter a value and returns it as a string. For example:

`intro_to_python.py`

```python
name = input("Enter your name: ")
print("Hello,", name)
# Prints: "Hello, Aya" (if the user enters Aya)
```

In this code, the `input()` function prompts the user to enter their name, and the entered value is stored in the name variable. The `print()` function is then used to display a greeting message and the user's name.

You can convert the user's input to a different data type if needed. For example, to convert the input to an integer, you can use the `int()` function:

`intro_to_python.py`

```python
age = int(input("Enter your age: "))
print("You are", age, "years old.")
```

## Operators

Python supports various operators that allow you to perform operations on variables and values. Here are some commonly used operators:

### Arithmetic operators

Arithmetic operators are used to perform mathematical operations on numbers. These include:

- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)

Here are some examples of arithmetic operations in action:

`intro_to_python.py`

```python
x = 10
y = 5

print(x + y)
# Prints: 15
print(x - y)
# Prints: 5
print(x * y)
# Prints: 50
print(x / y)
# Prints: 2.0
```

### Comparison operators

Comparison operators are used to compare two values and return a boolean result (True or False). These include:

- `==` (equal to)
- `!=` (not equal to)
- `>` (greater than)
- `<` (less than)
- `>=` (greater than or equal to)
- `<=` (less than or equal to)

Here's how you can use them:

`intro_to_python.py`

```python
print(x == y)
# Prints: False
print(x != y)
# Prints: True
print(x > y)
# Prints: True
print(x < y)
# Prints: False
print(x >= y)
# Prints: True
print(x <= y)
# Prints: False
```

### Logical operators

Logical operators are used to combine multiple boolean expressions and return a boolean result:

- `and` (logical AND)
- `or` (logical OR)
- `not` (logical NOT)

Here's an example that demonstrates the use of these operators:

`intro_to_python.py`

```python
print((x > 5) and (y < 10))
# Prints: True
print((x > 5) or (y > 10))
# Prints: True
print(not (x == y))
# Prints: True
```
