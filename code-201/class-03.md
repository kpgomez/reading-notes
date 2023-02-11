# Class 03
Date: 02/11/2023

## Learn HTML

### Order and Unordered Lists

global attributes; reversed, start, type which is now list-style-type, compact which is now line-height, 

Q&A

1. When should you use an unordered list in your HTML document? when the order of the items listed does not matter, there is no precedence, or the items do not have an ascending or descending value like a top ten list or worst of all time, etc.
2. How do you change the bullet style of an unordered list items? with an attribute list-style-type. list-style-type options includes "circle", "disc", or "square"
3. When should you use an ordered list vs an unordered list in your HTML document? when the order of the list has meaning
4. Describe two ways you can change the numbers on list items provided by an ordered list?


## Learn CSS - The Box Model

*Everything in CSS has an invisible box around it*

Block vs inline boxes

h1, p, list are by default block
a, span, em, strong are by default inline


All boxes have an inner or outer display type

attributes; display

Q&A

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled "The Box Model"? content Padding surrounds the contents and pushes it inward whereas margin helps separate or create space from other HTML elements
2. List and describe the four parts of an HTML elements box as referred to by the box model. Margin, padding, content and border. Content, the most inner part of the box mdoel, displays the content. The next layer that surrounds content is the padding. Padding pushes content more inward, I believe. The border wraps or contains the content and padding. The margin is the outermost layer and creates separation or distance from other elements. 

## Learn JS - Arrays, Operators and Expressions, Conditionals, Loops

Q&A
1. what data types can you store inside of an Array? strings, numbers, objects and other arrays
2. Is the people array a valid JavaScript array? yes. If so, how can I access the values stored? via its index [] indicates first level index, [][] indicates second level index or index of an array within an array
3. List five shorthand operators for assignment in javascript and describe what they do.

- += this adds the expression then reassigns the new value to - the variable
- -= this subtracts the expression then reassigns the new value to the variable
- *= this multiplies the expression then reassigns the new value to the variable
- /= this divides the expression then reassigns the new value to the variable
- %= this calculates the remainder or modulus of the expression then reassigns the that value to the variable

4. Read the code below and evaluate the last expression and explain what the result would be and why. console shows 10dog so the strings were concatenated. anything plus a string becomes a string????
5. Describe a real world example of when a conditional example of when a conditional statement should be used in a JavaScript program. for login credentials
6. Give an example of when a Loop is useful in JavaScript. when the same code needs to iterates over a large or even unknown number of times


# Things I want to know more about

- CSS [Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)
- Flexbox
- math to determine the actual space taken up by the box model
- alternative CSS box model