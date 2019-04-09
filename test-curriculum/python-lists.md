    title: Lists in Python
    author: John Smith
    date: 4/2/19
    next: [Step 2](@step_2.md) ///links not creating within "---"
    prev: [Intro](@intro.md)
    jump to: @step1.md
    
# Lists in Python
Lists are a great tool to map data to other data. Python's list are a way to organize your data. Your data would be structured like

![alt text](https://raw.githubusercontent.com/codingandcommunity/test-articles/master/test-curriculum/assets/python-list%20diagram.jpg "list diagram")a

You can create a List with a set of intial elements

```python
var numbers = [1, 2, 3];
colors = ["red", "blue", "red"]
data = ["red", 1, 1.5, true];
```
and an empty list

```python
numbers = []
```

The data in the List can be any type and all elements do not have to be the same type. If a single element is needed in the list it can be accessed using []; where a element is its element. Remember that the first element is the zeroth element.

```python
three = numbers[2]
```

In this case the number 3 is in the 2nd index of the list.


## Iteration
Going through every element in some in order or in some sequence is called iteration. It is very useful to *iterate* through a List. For example to add one to each number in a List or get the max number.

### For In Loop
One way to iterate through a list is a for in loop. For example, if we had a list of numbers called `numbers` we can print each number like so.

```python
for num in numbers:
  print(num)
```

The variable num is now a temporary variable that can only be used within that code block and is a element in the List `numbers`.

The `in` keyword can be use to check if something is in the list.

```python
if 2 in numbers:
	print '2 is in the list'
```

### For and while Loop

The list can also be iterated using indexes. The range function can be used to go through all numbers until the number specified. For example if we had a list of 100 numbers.

```python
for index in range(100):
	print numbers[index];
```

This prints out the 0th to 99th index of the numbers list. The range function can also start a different value and increment at diffenent values. `range(start,end,increment)`

```python
index = 0
while index < len(numbers):
	print numbers[index];
	i += 1;
```
This prints out every element of the list using a while loop and indexes to get specific elements. We can also increment at different values like this.

```python
index = 0
while index < len(numbers):
	print numbers[index];
	i += 2;
```

This will print every other or every even indexed element.

## Changing Lists

If we want to change our list `numbers` we use so functions.

* numbers.append(element) adds a element to the end of our list of numbers
* numbers.insert(index,elemnt) adds a element at the index essentially incrementing the elements' index by 1 after the inserted element.
* numbers.index(element) searches for the index of the element given.
* numbers.remove(element) searches and removes the element given. The indexes of the elements to the right of the removed elements will be decreased by one.
* numbers.pop(index) removes the element at the index given. The indexes of the elements to the right of the removed elements will be decreased by one.

There are more functions that can manipulate lists and would be beneficial to read about them and practice them by thinking about or looking at how the functions can be used.
You can read more [here](https://docs.python.org/3/tutorial/datastructures.html).



