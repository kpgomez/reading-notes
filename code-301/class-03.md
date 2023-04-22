## React Docs - lists and keys

[Source](https://legacy.reactjs.org/docs/lists-and-keys.html)
[New React Docs](https://react.dev/learn/rendering-lists)

**Notes**
a key is required for list items


*Syntax Example*

`const numbers = [1, 2, 3, 4, 5];`
`const listItems = numbers.map((numbers) =>`
  `<li>{numbers}</li>`
`);`

`const root = ReactDOM.createRoot(document.getElementById('root')); ` 

-> grabs html element with id 'root', which is then passed through ReactDOM.createRoot method turning it into a React Component and then that is assigned to a constant variable named 'root'

`root.render(<ul>{listItems}</ul>);`

"Keys serve as a hint to React but they don’t get passed to your components. If you need the same value in your component, pass it explicitly as a prop with a different name:"

JSX stands for JavaScript XML and allows dev to write HTML in React

XML is extensible markup language

**Q&A**
1. What does .map() return? It returns a new array
2. If I want to loop through an array and display each value in JSX, how do I do that in React? Use forEach() or map() method and include the returned value in {} (curly braces) indicating it is a JSX expression
3. Each list item needs a unique **key**.
4. What is the purpose of a key? to give each element inside of an array a stable identity

## The Spread Operator

[Source](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

**Notes**

`Math.max(1,3,5)` // 5
`Math.max([1,3,5])` // NaN

The spread operator is useful for ...
- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array


**Q&A**
1. What is the spread operator? `(...)` 
2. List 4 things that the spread operator can do. 
    1. Add items to an array
    2. Combine arrays
    3. Combine objects
    4. pread an array out into a function's arguments
3. Give an example of using the spread operator to combine two arrays.

`const array1 = [1, 2, 3];`
`const array2 = [4, 5, 6];`
`const combinedArray = [...array1,...array2]`

4. Give an example of using the spread operator to add a new item to an array.

`const array1 = [1, 2, 3];`
`const array2 = [4, 5, 6,...array1];`


5. Give an example of using the spread operator to combine two objects into one.

`const obj1 = {name: 'Napoleon'}`
`const obj2 = {name: 'Georgina'}}`
`const combinedObject = [...obj1,...obj2]`

Videos

## How to Pass Functions Between Components

[Source](https://www.youtube.com/watch?v=c05OL7XbwXU) <- this video was confusing

**Q&A**
1. In the video, what is the first step that the developer does to pass functions between components? Create the function whereever the state resides. In the video example, the function was created below the constructor
2. In your own words, what does the increment function do? increment the count by 1
3. How can you pass a method from a parent component into a child component? by using the 'this' keyword
4. How does the child component invoke a method that was passed to it from a parent component? this.methodName

### Bookmark and Review
[React Tutorial through ‘Declaring a Winner’](https://react.dev/learn/tutorial-tic-tac-toe)
[React Docs - Lifting State Up](https://legacy.reactjs.org/docs/lifting-state-up.html)

### For Further Review
[Intro to JSX](https://legacy.reactjs.org/docs/introducing-jsx.html#embedding-expressions-in-jsx)