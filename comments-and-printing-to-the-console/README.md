<h1>
  <span class="headline">Intro to Python for Scripting</span>
  <span class="subhead">Comments and Printing to the Console</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to contribute comments to Python code and print output to the console.

## Printing to the console

In Python, we use the `print()` function to print a message to the console:

`intro_to_python.py`

```python
print("Hello, world!")
```

This will output the string `Hello, world!` to the console.

Test this now by running the following command in your terminal to execute the file:

```bash
python3 intro_to_python.py
```

You should see the output `Hello, world!` in your terminal.

## Comments

Comments are an important part of scripting. They allow you to add notes and explanations to your code so that you and others can better understand it when you refer back to it later. The Python interpreter ignores these comments, so they don't affect the execution of your code.

In Python, comments are created using the `#` symbol. Everything after the `#` on that line is considered a comment and will be ignored by the interpreter. Add an explanation to the print statement in your `intro_to_python.py` file:

`intro_to_python.py`

```python
# Prints "Hello, world!" to the console
print("Hello, world!")
```

Typically, comments are used to explain the purpose of a block of code or to provide additional context. Code like `print("Hello, world!")` is self-explanatory, so it typically wouldn't need a comment; we're just using it as an example here.
