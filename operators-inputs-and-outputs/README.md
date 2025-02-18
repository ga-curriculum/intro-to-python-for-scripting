<h1>
  <span class="headline">Intro to Python for Scripting</span>
  <span class="subhead">Inputs, Outputs, Operators and Branching</span>
</h1>

**Learning objective:** By the end of this lesson, students will understand how python handles operators, as well as user input and output.

## User Input and Output

Python provides built-in functions to interact with the user and display output.

### User Input

To get input from the user, you can use the `input()` function. It prompts the user to enter a value and returns it as a string. For example:

``` python
name = input("Enter your name: ")
print("Hello,", name)
```

In this code, the `input()` function prompts the user to enter their name, and the entered value is stored in the name variable. The `print()` function is then used to display a greeting message along with the user's name.

You can convert the user's input to a different data type if needed. For example, to convert the input to an integer, you can use the `int()` function:

``` python
age = int(input("Enter your age: "))
print("You are", age, "years old.")
```

### Output

To display output, you can use the `print()` function. It takes one or more arguments and displays them on the console. For example:

``` python
print("Hello, World!")
print("The sum of 2 and 3 is", 2 + 3)
```

In the first line, the `print()` function displays the string `"Hello, World!"` on the console. In the second line, it displays a message along with the result of the expression `2 + 3`.

You can use various formatting techniques to control the appearance of the output. For example, you can use f-strings to embed variables or expressions within a string:

``` python
name = "Alice"
age = 25
print(f"My name is {name} and I am {age} years old.")
```


This will output: `"My name is Alice and I am 25 years old."`

## Operators

Python supports various operators that allow you to perform operations on variables and values. Here are some commonly used operators:

1. **Arithmetic Operators**

- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)

2. **Comparison Operators**

- `==` (equal to)
- `!=` (not equal to)
- `>` (greater than)
- `<` (less than)
- `>=` (greater than or equal to)
- `<=` (less than or equal to)

3. **Logical Operators**

- `and` (logical AND)
- `or` (logical OR)
- `not` (logical NOT)

Here's an example that demonstrates the use of operators:

``` python
x = 10
y = 5

print(x + y)  # Output: 15
print(x - y)  # Output: 5
print(x * y)  # Output: 50
print(x / y)  # Output: 2.0

print(x == y)  # Output: False
print(x != y)  # Output: True
print(x > y)  # Output: True
print(x < y)  # Output: False
print(x >= y)  # Output: True
print(x <= y)  # Output: False

print((x > 5) and (y < 10))  # Output: True
print((x > 5) or (y > 10))  # Output: True
print(not (x == y))  # Output: True
```
