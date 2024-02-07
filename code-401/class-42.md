# Class 42 - Pythonisms

## Notes
### Dunder methods
`__init__` constructor for object initialization \
`__str__` friendly object representation to the end-user through print() \
`__repr__` official string representation of the object \
`__len__` for iteration \
`__getitem__` for iteration \
`__reversed__` for iteration \
`__eq__` and `__lt__` operator overloading for comparisons \
`__add__` operator overloading for adding \
`__class__` \
`__name__`


## Readings
- [Dunder Methods](https://dbader.org/blog/python-dunder-methods)
- [Iterators](https://dbader.org/blog/python-iterators)
- [Generators](https://dbader.org/blog/python-generators)

## Videos
- [What are Generators](https://realpython.com/lessons/what-are-python-generators/)

## Bookmark and Review
- [Decorators](https://realpython.com/primer-on-python-decorators/)

## Reading Questions
1. What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.
> Dunder stands for "double under" score and it refers to all the magic methods in Python that begin and end with `__` such as `__name__`, `__main__`, `__init__`, and many more. Dunder methods let you emulate behavior of built-in types. `__new__` creates a new instance of class cls.
2. Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?
> An iterator returns an iterable. Iterable means you can iterate aka loop over a sequence. You can create a custom iterator by add `__iter__` and `__next__`to the class definition. According to the article, iterators are important because they provide a sequence interface to Python's objects that's memory efficient. 
3. What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.
> Per the article, generator functions are syntactic sugar for writing objects that support the iterator protocol. Unlike regular functions, generators use the keyword `yield` instead of `return`.

```python
def repeater(value):
    while True:
        yield value
```
4. Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.
> "A decorator is a function that takes another function and extends the behavior of the latter function without explicitly modifying it." 
> @ aka "pie" syntax applies the decorator to a function or method. 

```python
class Student:
    name = 'unknown' # class attribute
    
    def __init__(self):
        self.age = 20  # instance attribute

    @staticmethod
    def tostring():
        print('Student Class')
```

[Source](https://www.tutorialsteacher.com/python/staticmethod-decorator)

## Things I want to learn more about
- [Special method names](https://docs.python.org/3/reference/datamodel.html#special-method-names)
- [Iterator protocol](https://docs.python.org/3/c-api/iter.html#iterator-protocol)