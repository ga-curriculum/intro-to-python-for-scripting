<h1>
  <span class="headline">Intro to Python for Scripting</span>
  <span class="subhead"></span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand branching and loops within Python. 

## Branching

Branching allows you to make decisions in your code based on certain conditions. In Python, you can use the `if`, `elif` (else if), and `else` statements to create branching logic. Here's an example:

``` python
age = 18

if age < 18:
    print("You are a minor.")
elif age >= 18 and age < 65:
    print("You are an adult.")
else:
    print("You are a senior.")
```

In this code, the `if` statement checks if the age is less than 18. If it is, the corresponding block of code is executed, and the message `"You are a minor."` is printed. If the condition is not met, the `elif` statement checks if the age is between 18 and 64 (inclusive). If it is, the message `"You are an adult."` is printed. If none of the previous conditions are met, the `else` block is executed, and the message `"You are a senior."` is printed.

The `if`, `elif`, and `else` statements allow you to create branching paths in your code based on different conditions. You can have multiple `elif` statements to check for various conditions, and the `else` block is executed if none of the conditions are met.

Let's consider an example to solidify our understanding of branching. Imagine you're creating a simple grading system that assigns letter grades based on a student's score. Here's how you could implement it using branching:

``` python
score = 85

if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
elif score >= 60:
    grade = "D"
else:
    grade = "F"

print("Your grade is:", grade)
```

In this example, the `if` and `elif` statements check the student's score against different thresholds and assign the corresponding letter grade. The else block is used as a catch-all for scores below 60, assigning the grade "F".

Branching is a fundamental concept in programming that allows you to create dynamic and responsive code. It enables you to make decisions and execute different blocks of code based on specific conditions.

## Looping

Looping allows you to repeat a block of code multiple times. Python provides two types of loops: `for` loops and `while`loops.

### `for` Loop

The `for` loop is used to iterate over a sequence (such as a list, tuple, or string) or other iterable objects. It allows you to execute a block of code for each item in the sequence.

Let's look at an example to understand how `for` loops work. Suppose you have a list of fruits and want to print each fruit on a separate line. You can use a `for` loop like this:

``` python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```

In this example, the `for` loop iterates over each element in the `fruits` list. On each iteration, the current fruit is assigned to the variable `fruit`, and the `print()` function is used to display its value.

The output will be:

``` python
apple
banana
cherry
```

The `for` loop automatically handles the iteration for you, allowing you to focus on the code you want to execute for each item in the sequence.

You can also use the `range()` function in combination with a `for` loop to iterate over a sequence of numbers. For example:

``` python
for i in range(5):
    print(i)
```

In this case, the `range(5)` function generates a sequence of numbers from 0 to 4 (5 is not included), and the `for` loop iterates over each number. The output will be:

``` python
0
1
2
3
4
```

The `range()` function is commonly used when you need to perform a specific number of iterations or when you need to access the index of each item in a sequence.

### `while` Loop

The `while` loop is used to repeatedly execute a block of code as long as a given condition is true. It continues to execute until the condition becomes false.

Here's an example to illustrate the usage of a `while` loop. Let's say you want to print the numbers from 1 to 5 using a `while` loop. You can do it like this:

``` python
count = 1

while count <= 5:
    print(count)
    count += 1
```

In this example, the `while` loop continues to execute as long as the count variable is less than or equal to 5. Inside the loop, the current value of `count` is printed, and then `count` is incremented by 1 using the `+=` operator.

The output will be:

``` python
1
2
3
4
5
```

The `while` loop is useful when you don't know beforehand how many times you need to iterate, and you want to continue executing a block of code until a certain condition is met.

**Tip** Be cautious when using while loops to avoid infinite loops. Make sure the condition eventually becomes false; otherwise, the loop will continue indefinitely, causing your program to hang.

## Loop Control Statements

In addition to the basic loop structures, Python provides control statements that allow you to modify the behavior of loops. Let's explore two commonly used loop control statements: `break` and `continue`.

### `break` Statement

The `break` statement is used to prematurely exit a loop. When encountered, it immediately terminates the loop and transfers the control to the next statement after the loop.

Let's consider an example where you want to find the first occurrence of a specific number in a list. You can use a `for` loop with a `break` statement like this:

``` python
numbers = [1, 3, 5, 7, 9, 2, 4, 6, 8]
search_number = 7

for number in numbers:
    if number == search_number:
        print(f"Found {search_number} in the list!")
        break
```

In this example, the `for` loop iterates over each number in the numbers list. When the `search_number` (7) is found, the `print()` function is executed, and the `break` statement is encountered. This immediately terminates the loop, and the program continues with the next statement after the loop.

The output will be:

``` python
Found 7 in the list!
```

The `break` statement is useful when you want to stop the loop execution as soon as a certain condition is met, saving unnecessary iterations.

### `continue` Statement

The `continue` statement is used to skip the rest of the current iteration and move to the next iteration of the loop.

Let's say you want to print all the numbers from 1 to 10, except for the number 5. You can use a `for` loop with a `continue` statement like this:

``` python
for i in range(1, 11):
    if i == 5:
        continue
    print(i)
```

In this example, the `for` loop iterates over the numbers from 1 to 10 (inclusive). When the loop encounters the number 5, the `if` condition is true, and the `continue` statement is executed. This skips the rest of the code block for that iteration (in this case, the `print()` function) and moves to the next iteration.

The output will be:

``` python
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

**Tip** Use loop control statements judiciously to maintain the readability and clarity of your code. Overusing them can make your code harder to understand and debug.


