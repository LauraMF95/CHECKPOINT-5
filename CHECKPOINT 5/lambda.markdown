# WHAT IS A LAMBDA FUNCTION IN PYTHON?

A **lambda function** is a tool that allows you to wrap up a function. Usually, a smaller function and 
then easily pass it to other functions. Now functions inside of python are what are called first-class 
citizens which means that you can treat a function like any type of object.

And so when we're working with Lambda's what we can do is wrap up some behavior, usually pretty small 
behavior and then pass it to other functions. So they are very mobile easy to use if you want one way of 
thinking about them you can take the perspective that a lambda is a very similar almost to a variable 
where you can pass in instead of some basic kind of values such as a string or a dictionary or something 
like that.

A lambda actually allows you to wrap up a process and so what we're going to do is we're going to place 
an ordinary function and then we will see how we can transform it into a lambda function.

## Ordinary function

This will be our initial function before we make it a lambda function. Is a *greeting* function that has 
two arguments (*first*, *last*), which will print a formatted greeting with the name and surname placed when we call the function:

```python
def greeting(first, last):
    print(f'Hi there {first} {last}')

greeting('Kristine', 'Hudgens')
```

## Lambda function

The basic syntax for it is going to be *full name* and that is what we're going to do a lambda returns 
of value so you're pretty much always going to be using a lambda where you're returning something. So 
we're going to return a full name value and we're going to store it inside of this full name variable.

So we're going to say *full name* equals and in order to create a lambda, you just say Lambda. So spell 
it out l a m b d a, followed by the list of arguments so we're simply going to pass in a first name and 
a last name and then pass a colon. And so this is going to be our set of function arguments that we're 
going to pass to Lambda and then whatever comes after the colon is going to be the value that is 
returned.

```python
full_name = lambda first, last: f'{first} {last}'

def greeting(name):
  print(f'Hi there {name}')

greeting(full_name('Kristine', 'Hudgens'))
```

So in review a Lambda gives you the ability to quickly and easily wrap functionality, store it in a 
variable and then pass that entire process to other functions and other parts of your program.
