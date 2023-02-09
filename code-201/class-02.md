# Class 02
Date: *02/07/2023*

## HTML Text Fundamentals

[Source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)
### Basic Rules
- each paragraph has to be wrapped in a p element
- each heading has to be wrapped in a heading element

### Best Practices

- one h1 tag per page
- use headings in the same order as its hierarchy
- no more than 3 heading levels per page
- use the right element for the right job
- make sure the structure makes sense

## HTML Advanced Text Formatting
[Source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

### Q&A
1. Why is it important to use semantic elements in our HTML? SEO rankings, screen readers, and user readability
2. How many levels of headings are there in HTML? six
3. What are some uses for the sup and sub elements? exponentiation and logarithms
4. When using the abbr element, what attribute must be added to provide the full expansion of the term? title


## How CSS is Structured
[Source](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

### Q&A
1. What are ways we can apply CSS to our HTML? inline, internal, external
2. Why should we avoid using inline styles? best practice is to use external CSS stylesheet
3. Review the block of code below and answer the following questions:
    &nbsp;1. What is representing the selector? h2 <br>
    &nbsp;2. Which components are the CSS declarations? element name, open/close curly brackes {}, and the arguments/parameters ---- color and padding <br>
    &nbsp;3. Which components are considered properties? black and 5px

## Javascript Basics Cont'd
[Source](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

**The return statement tells the browser to return the result variable out of the function so it is available to use outside of that particular funtion**

### Events

document.querySelector("html") // selects html element

.addEventListener("click", function()) // runs the function() specified in the event of a user's mouse click

function() above as specified is called an *anonymous function*

.addEventListener("click", ()) // uses an Arrow function which is the () by itself

### Q&A
1. What data type is a sequence of text enclosed in single quote marks? string
2. List 4 types of JavaScript operators. =, +, -, <, >, +=, <=, *, /
3. Describe a real world problem you could solve with a Function. I have to think about this one for a bit.

### Making Decisions in Your Code - Conditionals
[Source](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

if...else // else statement is optional but good practice since you want either code blocks to run not both

else if // a "way to chain on extra choices/outcomes". 


a conditional statement could be "does this value exist?" 

when function is declared as an argument, no need to use () such as select.addEventListener('change', setWeather) exmaple

**any value that is not *false*, *undefined*, *null*, *0*, *NaN*, or an *empty string* ('') returns true**

### switch statements

- take a single expression/value as input and executes the code block that matches the case

syntax of switch statement <br>

switch (expression) { case choice1: run this code; break; case choice2: run this code instead; break; default: run this code if no match is found}

### Q&A
1. An if statement checks a **condition** and if it evaluates to **true**, then the code block will execute.
2. What is the use of else if? to nest multiple conditions
3. List 3 different types of comparison operators. >, <, ===
4. What is the difference between the logical operator && and ||. && represents AND meaning both conditions must equal true for the set of condition to be true. || represents OR meaning if either condition is true, then that entire conditional statement is true.

[Git Commit - Bookmark and Further Review](https://cbea.ms/git-commit/)

### Things I want to know more about
- SEO
- DOM API
- *return* statement
- [variable scoping](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#variable_scope)
- document methods such as .querySelector, etc
- null values
- since everything in JavaScript is an object, does that mean they all share the same methods?
- *anonymous functions*
- [Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API)
- why is JavaScript syntax so lax...
- .onclick //
- .getAttribute // 
- .setAttribute // 
- .textContent //
- select.value //
- HTML *select* element
- .innerHTML vs .textContent
- syntax for nesting if...else 
- syntax of a conditional statement using the Ternary operator (?)