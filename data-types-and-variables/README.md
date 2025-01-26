<h1>
  <span class="headline">Intro to Python</span>
  <span class="subhead"> Data Types and Variables in Python</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand python data types and variables.

## Data Types in Python

Python has several built-in data types that you can use to represent different kinds of values. Let's take a closer look at some commonly used data types:

1. **Numbers**

- Integer(`int`): Represents whole numbers, such as `-5`, `0`, `42`.
- Float (`float`): Represents decimal numbers, such as `3.14`, `-2.5`, `1.0`.

2. **Strings**

- String (`str`): Represents a sequence of characters, enclosed in single quotes (`'...'`) or double quotes (`"..."`).
  - Examples: `"Hello, World!", 'Python is awesome'`

3. **Booleans**

- Boolean (`bool`): Represents a truth value, either `True` or `False`.

4. **Sequences**

- List (`list`): An ordered, mutable collection of elements, enclosed in square brackets (`[...]`).

  - Example: `[1, 2, 3, 4, 5]`

- Tuple (`tuple`): An ordered, immutable collection of elements, enclosed in parentheses (`(...)`).

  - Example: `(1, 2, 3, 4, 5)`

5. **Mappings**

- Dictionary (`dict`): An unordered collection of key-value pairs, enclosed in curly braces (`{...}`).

  - Example: `{"name": "Alice", "age": 25}`

Python is a dynamically-typed language, which means that you don't need to explicitly specify the data type of a variable. Python infers the data type based on the value assigned to the variable.

You can use the `type()` function to check the data type of a variable or value. For example:

``` python
print(type(42))  # Output: <class 'int'>
print(type("Hello"))  # Output: <class 'str'>
print(type(3.14))  # Output: <class 'float'>
```

Understanding data types is crucial for writing effective Python code. Different data types have different properties and behaviors, and you'll often need to convert between types or perform type-specific operations.

## Variables

Variables are used to store and manipulate data in Python. They act as containers that hold values of different types, such as numbers, strings, or more complex objects. In Python, you don't need to explicitly declare the type of a variable; Python infers it based on the value assigned.

### Creating Variables

To create a variable in Python, you simply choose a name for the variable and use the assignment operator (`=`) to assign a value to it. For example:

``` python
name = "Alice"
age = 25
height = 1.75
```

In the above code, we create three variables: `name` (a string), `age` (an integer), and `height` (a floating-point number).

Python has some rules and conventions for variable names:

- Variable names can contain letters (a-z, A-Z), digits (0-9), and underscores (_).

- Variable names must start with a letter or an underscore.

- Variable names are case-sensitive (`myVariable` and `myvariable` are different variables).

- Avoid using reserved keywords as variable names (e.g., `if`, `for`, `while`).

- Choose descriptive and meaningful names that reflect the purpose of the variable.

### Accessing Variables

To access the value of a variable, you simply use its name. You can use variables in expressions, print their values, or pass them as arguments to functions. For example:

``` python
print(name)  # Output: Alice
print("Age:", age)  # Output: Age: 25
print("Height:", height)  # Output: Height: 1.75
```

## Practice: Variables and Data Types

Let's reinforce our understanding of variables and data types with a few practice exercises. Try solving these exercises on your own and then compare your solutions with the provided answers.

1. Create a variable called `favorite_color` and assign it a string value representing your favorite color. Print the value of `favorite_color`.

2. Create two variables, `x` and `y`, and assign them numeric values. Calculate their sum and store the result in a new variable called `sum`. Print the value of `sum`.

3. Create a variable called `is_raining` and assign it a boolean value representing whether it is currently raining or not. Print the value of `is_raining`.

4. Create a list called `fruits` and add three of your favorite fruits as strings to the list. Print the contents of the `fruits` list.

5. Create a dictionary called `person` with keys "name", "age", and "city", and assign appropriate values to each key. Print the value of the "name" key.

Take a moment to work on these exercises and then compare your solutions with the following:

``` python
# Exercise 1
favorite_color = "blue"
print(favorite_color)

# Exercise 2
x = 10
y = 5
sum = x + y
print(sum)

# Exercise 3
is_raining = False
print(is_raining)

# Exercise 4
fruits = ["apple", "banana", "orange"]
print(fruits)

# Exercise 5
person = {"name": "Alice", "age": 25, "city": "New York"}
print(person["name"])
```

Practice is key to becoming comfortable with variables and data types in Python. Don't hesitate to experiment and try out different variations of these exercises to deepen your understanding.