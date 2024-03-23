# CONDITIONALS

## What is a conditional?

In computer science, **conditionals** (that is, conditional statements, conditional expressions and conditional constructs) are programming language commands for handling decisions. Specifically, conditionals perform different computations or actions depending on whether a programmer-defined Boolean condition evaluates to true or false. In terms of control flow, the decision is always achieved by selectively altering the control flow based on some condition (apart from the case of branch predication). Although dynamic dispatch is not usually classified as a conditional construct, it is another way to select between alternatives at runtime. Conditional statements are the checkpoints in the programme that determines behaviour according to situation.

A conditional is one of the foundational concepts around what it takes to make a python program become dynamic. By dynamic what I mean is that your program can start making decisions which is a pretty exciting and very cool feature that pretty much every type of application is going to have to have at some level or another. Now conditionals are simply a way of saying if one situation occurs I want you as a program to perform one task but if a different situation occurs I want you to perform this other task.

## Python Conditions and If statements

Python supports the usual logical conditions from mathematics:

- **Equals**: a == b
- **Not Equals**: a != b
- **Less than**: a < b
- **Less than or equal to**: a <= b
- **Greater than**: a > b
- **Greater than or equal to**: a >= b

These conditions can be used in several ways, most commonly in "if statements" and loops.

An "if statement" is written by using the if keyword.

Example:

```python
a = 15
b = 400
if b > a:
  print("b is greater than a")
```

In this example we use two variables, a and b, which are used as part of the if statement to test 
whether b is greater than a. As a is 15, and b is 400, we know that 200 is greater than 33, and so we 
print to screen that "b is greater than a".

## Indentation

Python relies on indentation (whitespace at the beginning of a line) to define scope in the code. Other 
programming languages often use curly-brackets for this purpose. If you place it without indentation, it 
will raise an error.

## Elif

The elif keyword is Python's way of saying "if the previous conditions were not true, then try this 
condition".

Example:

```python
a = 27
b = 27
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```

In this example a is equal to b, so the first condition is not true, but the elif condition is true, so 
we print to screen that "a and b are equal".

## Else

The else keyword catches anything which isn't caught by the preceding conditions.

Example:

```python
a = 151
b = 12
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```

In this example a is greater than b, so the first condition is not true, also the elif condition is not 
true, so we go to the else condition and print to screen that "a is greater than b".
You can also have an else without the elif.

## Ternary operators

The Python ternary operator determines if a condition is true or false and then returns the appropriate 
value in accordance with the result. The ternary operator is useful in cases where we need to assign a 
value to a variable based on a simple condition, and we want to keep our code more concise — all in just 
one line of code. It’s particularly handy when you want to avoid writing multiple lines for a simple 
if-else situation.

Example:

```python
role = 'guest'

auth = 'can access' if role == 'admin' else 'cannot access'
```

## Compound conditionals

Compound conditionals set multiple conditions inside of a python program. There are 3 operators with 
whom we can make them:

- **AND**: in order to be true, both parts of the conditionals must be true.

Example:

```python
a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
```

- **OR**: in order to be true, one part or the other of the conditional must be true.

Example:

```python
a = 200
b = 33
c = 500
if a > b or a > c:
  print("At least one of the conditions is True")
```

- **AND NOT**: in order to be true, one part of the conditional must be true and the other false.

Example:

```python
a = True
b = False
if a and not b:
  print("One condition is True and the other is False")
```
