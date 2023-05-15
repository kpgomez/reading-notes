## Understanding the JavaScript Call Stack

[Source](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’? a function invocation
2. How many ‘calls’ can happen at once? one
3. What does LIFO mean? Last in First Out
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
![Example](./Screenshot%202023-05-14%20at%208.24.22%20PM.png)
5. What causes a Stack Overflow? When a function calls itself

## JavaScript error messages

[Source](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

**Notes**

const, let are hoisted like var and function but there is a time between hoisting and declaration that can lead to a Temporal Dead Zone

1. What is a ‘reference error’? when you try to use a variable that has not been declared
2. What is a ‘syntax error’? when there is a syntax issue
3. What is a ‘range error’? can refer to invalid length
4. What is a ‘type error’? when the variable type is incompatible or undefined
5. What is a breakpoint? an area  in the code that is designated testing of some sort
6. What does the word ‘debugger’ do in your code? it's a conditional breakpoint

## Bookmark and Review

[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)