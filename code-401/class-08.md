## Class 08

The following readings and videos are important because Python's comprehension features increase its readability and enhance 

## Sources
- [List Comprehension](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
- [Debugging with PySnooper](https://www.pythonpodcast.com/pysnooper-python-debugging-episode-241/)


## List Comprehension Notes

### syntax for list comprehension

![Alt text](image-9.png)

starting backwards

iterable_object refers to anything iterable meaning you can loop through it such as list, tuple, set, string, **FILES**  .....

item refers to element in the iterable_object

expression represents the operation that is performed on each element or item in the iterable object

the result of the list comprehension is assigned to my_new_list

*How does the comprehensions compare to arrow functions in JavaScript?*

- [Python comprehensions vs JavaScript arrow functions - ChatGPT explanation](https://chat.openai.com/c/ae6d1b18-6b01-4020-aed8-1ebb23bdab04)

### Example

![Alt text](image-10.png)

### Adding conditional expressions

Syntax

`my_new_list = [ expression for item in iterable_object conditional statement/evaluation]`

functions are added to the expression

Examples

![Alt text](image-15.png)

![Alt text](image-12.png)

Conditional statements act as a **filter**



### The Beauty of List Comprehensions

![Alt text](image-13.png)

### More Examples

![Alt text](<Screenshot 2023-10-10 at 3.50.53 PM.png>)

### Useful example to apply to webscraping output possibly ...

![Alt text](<Screenshot 2023-10-10 at 3.55.18 PM.png>)

### Parsing a File

![Alt text](image-14.png)

### Delimiters

<hr>

## Primer on Python Decorator Notes

A decorator is a function that takes another function and extends the behavior of the second function

Functions are first-cass objects that can be passed around and used as arguments

When a function is named without parentheses, only the reference to the function is passed and the function is not executed

`greet_bob(say_hello)`

say_hello is a reference

inner functions are functions defined inside other functions and are locally scoped to the enclosing function

![Alt text](<Screenshot 2023-10-10 at 7.15.27 PM-1.png>)

### Returning Functions from Functions

![Alt text](<Screenshot 2023-10-10 at 7.15.27 PM.png>)


## PySnooper
1. pip install PySnooper
2. import PySnooper
3. add snooper.pysnooper decorators


## Bookmark and Review
- [Primer on Decorators](https://realpython.com/primer-on-python-decorators/)

## Reading Questions

1. What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.

*syntax as follows*

variable = [expression for item in iterable_objection conditional statement]

*example of list comprehension* 

`numbers = [2, 4, 8, 12]`

`squared = [num**2 for num in numbers]`

![Alt text](image-11.png)

2. What is a decorator in Python? a function that extends another function

3. Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.

![Alt text](image-16.png)

## Things I Want to Learn More About
- Are comprehensions algorithmically more efficient?
- [String Indexing](https://www.pythonforbeginners.com/strings/string-indexing-in-python)
- [Dictionary Comprehension](https://www.pythonforbeginners.com/dictionary/dictionary-comprehension-in-python)
- [String Concatenation](https://www.pythonforbeginners.com/concatenation/string-concatenation-and-formatting-in-python)
- [Iterators & Iterables](https://realpython.com/python-iterators-iterables/)
- Rust
- Fintech
- [PySnooper](https://github.com/cool-RR/PySnooper/?utm_source=rss&utm_medium=rss)
- [Wing IDE](https://wingware.com/?utm_source=rss&utm_medium=rss)
- [Higher-order functions](https://en.wikipedia.org/wiki/Higher-order_function)
- [Functional Programming in Python](https://realpython.com/python-functional-programming/)