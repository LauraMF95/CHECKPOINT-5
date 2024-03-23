# WHAT IS AN ARGUMENT IN PYTHON

Information can be passed into functions as arguments.
Arguments are specified after the function name, inside the parentheses. You can add as many arguments 
as you want, just separate them with a comma.
The following example has a function with one argument (name). When the function is called, we pass 
along a first name, which is used inside the function to print the full name:  

Example:

```python
def my_function(name):
  print(full_name + "worker")

my_function("Sara")
```

## Number of arguments

By default, a function must be called with the correct number of arguments. Meaning that if your 
function expects 2 arguments, you have to call the function with 2 arguments, not more, and not less.

Example:

```python
def my_function(first_name, last_name):
  print(first_name + " " + last_name)

my_function("Sara", "Mittens")
```

## Types of arguments

There are two types of arguments in Python: positional arguments and keyword arguments.

- **Positional arguments**: they are passed to a function, method, or class in the order that they are 
defined. 

- **Named arguments**: named arguments (or keyword arguments) are values that, when passed into a 
function, are identifiable by specific parameter names. A named argument is preceded by a parameter and 
the assignment operator, = . Keyword arguments can be likened to dictionaries in that they map a value 
to a keyword. Example:

```python
def team(name, project):
    print(name, "is working on an", project)

team(project = "Answers", name = 'FemCode')
```

## Default arguments

Default values indicate that the function argument will take that value if no argument value is passed 
during the function call. The default value is assigned by using the assignment(=) operator of the form 
keywordname=value.

Let’s understand this through a function *greeting*. In the first case, as the name is placed, it will print *Hi Kristine*, as we expect. However, in the second case it will print *Hi Guest*, cause in *greeting* fuction we don't place anything and it will take the default argument *Guest*. 

```python
def greeting(name = 'Guest'):
  print(f'Hi {name}!')

greeting('Kristine')
greeting()
```
