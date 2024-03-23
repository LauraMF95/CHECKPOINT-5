# LOOPS

Looping means repeating something over and over until a particular condition is satisfied. A for loop in 
Python is a control flow statement that is used to repeatedly execute a group of statements as long as 
the condition is satisfied.

## What are the different types of loops in Python?

There are two ways to create loops in Python: with the **For In LOOP** and the **While LOOP**.

## FOR IN LOOP

A **for in loop**  is probably one of the most popular options and you're most likely going to be using it for the majority of your own Python programs.

For In-loops are used when you have a block of code which you want to repeat a **fixed number of times**. 
It is always used in combination with an iterable object, like a list or a range. The Python 
for statement iterates over the members of a sequence in order, executing the block each time.

An example of a For In-loop is the following one:

```python
players = ['Altuve', 'Bregman', 'Correa', 'Gattis']
for player in players:
  print(player)
```

## WHILE LOOP

Contrast of for in loop, a **while loop** will not stop when it reaches the end of a list if that's what you're iterating over a while loop has to explicitly be told when to stop and it's part of the reason why you would not want to use a while loop on a regular basis because there are many times where you might forget to tell the while loop to stop at a certain point and then you reach what is called an infinite loop which is something that can crash your program because the while loop will not stop until it has been told to stop and so you have to be able to define what that point is and just if you're interested in the formal term it's called a sentinel value. You have to set a **sentinel value** in order to tell your while loop when to stop.

An example of while loop is the following one:

```python
nums = list(range(1, 100))
while len(nums) > 0:
  print(nums.pop())
```

In this case, what is going to happen is that it's going to iterate over a list, it's going to pop 
an element off and it's going to print out that value. If you remember the behavior of the **pop function** this will also remove the item from the names list, so this is going to create our **sentinel value**. It's going to continually decrease the length of the nums list until it reaches 0, once it 
reaches that value. When this happens, the condition is going to be false and when it's false the while 
loop is going to stop.

To finish with, one of the most common uses for a while loop is when you don't know how many times you 
want your program to iterate. If you do know, you will prefer to use the for in loop.
