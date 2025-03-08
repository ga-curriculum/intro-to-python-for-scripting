<h1>
  <span class="headline">Intro to Python for Scripting</span>
  <span class="subhead"></span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to apply Python's `for` and `while` statements to implement conditional looping logic in a script.

## Looping

Looping allows you to repeat a block of code multiple times. Python provides two types of loops: `for` loops and `while` loops.

### `for` loop

The `for` loop iterates over a sequence (such as a list, tuple, or string) or other iterable objects. It allows you to execute a block of code for each item in the sequence.

Let's look at an example to understand how `for` loops work. Suppose you have a list of fruits and want to print each fruit on a separate line. You can use a `for` loop like this:

`intro_to_python.py`

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```

In this example, the `for` loop iterates over each element in the `fruits` list. On each iteration, the current fruit is assigned to the variable `fruit`, and the `print()` function displays its value.

The output will be:

```plaintext
apple
banana
cherry
```

The `for` loop automatically handles the iteration for you, allowing you to focus on the code you want to execute for each item in the sequence.

You can also use the `range()` function in combination with a `for` loop to iterate over a sequence of numbers. For example:

`intro_to_python.py`

```python
for i in range(5):
    print(i)
```

In this case, the `range(5)` function generates a sequence of numbers from 0 to 4 (5 is not included), and the `for` loop iterates over each number. The output will be:

```plaintext
0
1
2
3
4
```

The `range()` function is commonly used when you need to perform a specific number of iterations or when you need to access the index of each item in a sequence.

### `while` loop

The `while` loop is used to repeatedly execute a block of code as long as a given condition is true. It continues to execute until the condition becomes false.

Here's an example to illustrate the usage of a `while` loop. Let's say you want to print the numbers from 1 to 5 using a `while` loop. You can do it like this:

`intro_to_python.py`

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

In this example, the `while` loop continues to execute as long as the count variable is less than or equal to 5. Inside the loop, the current value of `count` is printed, and then `count` is incremented by 1 using the `+=` operator.

The output will be:

```plaintext
1
2
3
4
5
```

The `while` loop is useful when you don't know beforehand how many times you need to iterate and want to continue executing a block of code until a specific condition is met. For example, you might want to keep asking a user for input until they provide a valid response.

> ⚠️ Be cautious when using while loops to avoid infinite loops. Ensure the condition eventually becomes false; otherwise, the loop will continue indefinitely, causing your program to stop responding.

## Loop control statements

In addition to the basic loop structures, Python provides control statements that allow you to modify the behavior of loops. Let's explore two commonly used loop control statements: `break` and `continue`.

### `break` statement

The `break` statement is used to exit a loop prematurely. When encountered, it immediately terminates the loop and transfers the control to the next statement after the loop.

Let's consider an example where you want to find the first occurrence of a specific number in a list. You can use a `for` loop with a `break` statement like this:

`intro_to_python.py`

```python
numbers = [1, 3, 5, 7, 9, 2, 4, 6, 8]
search_number = 7

for number in numbers:
    if number == search_number:
        print(f"Found {search_number} in the list!")
        break
    else
        print(f"Found {number}, but it wasn't what we were looking for...")
```

In this example, the `for` loop iterates over each number in the numbers list. When the `search_number` (7) is found, the `print()` function is executed, and the `break` statement is encountered. This immediately terminates the loop, and the program continues with the next statement after the loop.

The output will be:

```plaintext
Found 1, but it wasn't what we were looking for...
Found 3, but it wasn't what we were looking for...
Found 5, but it wasn't what we were looking for...
Found 7 in the list!
```

Note that no more numbers are printed after the `Found 7 in the list!` message because the `break` statement terminated the loop. The `break` statement is useful when you want to stop the loop execution when a specific condition is met, saving unnecessary iterations.

### `continue` statement

The `continue` statement is used to skip the rest of the current iteration and move to the next iteration of the loop.

Let's say you want to print all the numbers from 1 to 10 except for the number 5. You can use a `for` loop with a `continue` statement like this:

``` python
for i in range(1, 11):
    if i == 5:
        continue
    print(i)
```

In this example, the `for` loop iterates over the numbers from 1 to 10 (inclusive). When the loop encounters the number 5, the `if` condition is true, and the `continue` statement is executed. This skips the rest of the code block for that iteration (in this case, the `print()` function) and moves to the next iteration.

The output will be:

```plaintext
1
2
3
4
6
7
8
9
10
```

The `continue` statement is useful when you want to skip specific iterations based on a certain condition without terminating the entire loop.

> 🧠 Use loop control statements judiciously to maintain the readability and clarity of your code. Overusing them can make your code harder to understand and debug.

<div class="activity solo-exercise">
  <h2 class="title">Are you sure you should go through the traffic signal?</h2>
  <span class="minutes">5 min</span>
</div>

Wrap the code you wrote in the previous branching exercise in a `while` loop.

- At the start of the loop, prompt the user to provide a color.
- If the user enters `green`, `yellow`, or `red`, the existing corresponding message should print, and the loop should run again.
- If the user enters `quit`, print `"Goodbye!"` and exit the loop.
- Nothing should be printed if the user enters anything else, but the loop should run again.
