#  WHAT IS LIST COMPREHENSION IN PYTHON

**List Comprehension** offers a shorter syntax when you want to create a new list based on the values of 
an existing list.

Example:

Based on a list of numbers, you want a new list, containing the numbers in the range from 1 to 10, all of them cubed:

```python
num_list = range(1, 11)
cubed_nums = []

for num in num_list:
  cubed_nums.append(num ** 3)
```

With list comprehension you can do all that with only one line of code:

```
cubed_nums = [num ** 3 for num in num_list]
```

## Syntax

In review, what we have here is a set of three different components essentially:
 
1. The first component is the actual value that we're wanting to do: *num ** 3*. This is the behavior we're wanting to implement, that in this case it is cubing whatever the number is. 

2. The second component is whatever expression you're wanting to run, your typical for in expression. So here we have *for num in num_list*. This is literally identical to copy and paste for the start of the for-in loop so that is what you have here for num in num_list.

3. The third component is the wrapper. So your parens or your square brackets that go around this entire expression. This is what tells Python that you don't just want to do a for-in loop for the cubed items you also want to dynamically generate a list and so that is what you're doing when you're wrapping this in brackets.
