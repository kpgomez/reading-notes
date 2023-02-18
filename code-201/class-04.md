# Class 04

Date: 02/14/2023

## Learn HTML - Creating Hyperlinks
[Source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

Q&A
1. To create a basic link, we wrap text or other content inside what element? a or anchor element
2. The href attribute contains what information? Hypertext reference or destination's web address
3. What are some ways we can ensure links on our page are accesible to all readers? By putting the title in regular text

## CSS Layout: Normal Flow CSS Layout
[Source](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

Absolute Units: 
- px or pixels, absolute, 1/96 of an inch
- mm or milliments, absolute, 1/10 of a cm
- pt or points, absolute, 1/72 of an inch


Relative Units:
- % or percentage of its default value relative to some other value (mainly based on the element's containing block)
-

## CSS Layout - Positioning

Position values; static (default), relative, or absolute (sits on its own layer and the position values specify distance from the each of the containing element's sides)

CSS rules
positioned: 
top: pushes down
bottom: pushes up
left: pushes content to the right
right: pushes content to the left

Relative's final position can be modified


Q&A
1. What is meant by "normal flow"? It is the *default* document flow
2. What are a few differences betwen block-level and inline elements? Block-level elements have an implicit newline character and take up the entire width of the page whereas inline elements only take up minimal amount of space and there is no implicit newline character
3. **Static** positioning is the default for every html element.


## Learn JS: Functions - Reusable Blocks of Code
[Source](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)

Built-in functions are defined in the browswer.
Custom functions are defined in your code.

.join() takes an array, joins all the array items together into a single string, and returns a new string

.replace('original string', 'revised string') string function takes a source string replacing it with a target string and returns a newly formed string (?)

you can specify default values by adding = after the name of the parameter, followed by the default value

anonymous no -name functions are useful when a function needs to take in another function as its parameter

function expressions are not hoisted meaning it must be defined before it can be used unlike normal functions which are hoisted

Q&A
1. Describe the difference between a function declaration and a function invocation. A function declaration has the let keyword whereas the function invocation does not.
2. What is the difference between a parameter and an argument? An argument is part of the function declaration and a parameter is part of the function invocation??? 


## Miscellaneous - 6 Reasons for Pair Programming

Q&A

1. Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.

Learning from fellow students will expose me to different approaches and perspectives to problem-solving in code. I might gain a new understanding or help point out concepts I don't fully understand so I can reserve time to build on it separately. 

Social skills. I can be a bit of a micro manager, and pair programming could help me learn how to try not to control everything. 

## Things I want to know more about
- Built-in browser functions and APIs
- what does low-level system language actually mean?
- [Built-in functions and objects and their corresponding methods ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)
- Identifying the containing block
- arrow functions
