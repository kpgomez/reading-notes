## React Docs - Thinking in React

[Source](https://react.dev/learn/thinking-in-react)

Example of breaking the UI into a component hierarchy
![Screenshot](./Screenshot%202023-04-29%20at%2010.09.07%20AM.png)


1. What is the single responsibility principle and how does it apply to components? responsibility refers to reason to change so in this case each component should contain at most a single state
2. What does it mean to build a ‘static’ version of your application? A version that renders the UI without any interactivity
3. Once you have a static application, what do you need to add? state
4. What are the three questions you can ask to determine if something is state? 
    1. Does it change over time?
    2. Is it passed in?
    3. Can you compute it based on existing state or props in your component?
5. How can you identify where state needs to live? Identify components that use state and find their common parent

## Higher-Order Functions

[Source](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”? Functions that operate on other functions
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing? returning the value that is greater of the two values
3. Explain how either map or reduce operates, with regards to higher-order functions. Map is a function that receives an array and another function and performs that received function on each element of the received array 