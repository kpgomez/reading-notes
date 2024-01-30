# Class 37: React 1

## Quickstart Notes

A component makes up the UI. Each component has its own logic and appearance. Each component contains JavaScript function that return markup (HTML).

Component types
- class
- functional

Rules
- React components start with a capital letter
- html tags are lower case

JSX (JavaScript Extension Syntax) is stricter than HTML. There are no self closing tags. All tags must end with />

className refers to CSS class. use quotes to pass in attributes. use curly braces to pass in javascript variables. can also use conditionals to specify attributes

{{}} indicate a javascript object passed as a variable

```javascript
function MyButton() {
    return (
        <> {/*empty frag*/}
        </>
    )
}
```

```javascript
export default function MyApp() {
    return (
        <div>
            <h1>Welcome to my app</h1>
            <MyButton /> {/*React Component*/}
        </div>
    )
}
```

```javascript
return (
    <>
        <img
            className="avatar"
            src={user.imageUrl}
            style={{
                width: user.imageSize,
                height: user.imageSize
            }}
        >
    </img>
)
```

export default (specifies the main component in the file ) vs export

<u>**conditional rendering**</u>

```javascript
let content;
if (isLoggedIn) {
    content = <AdminPanel />;
} else {
    content = <LoginForm />
}
return (
    <div>
        {content}
    </div>
);
```

<u>**ternary example**</u>

```javascript
<div>
    {isLoggedIn ? (
        <AdminPanel />
    ) : (
        <LoginForm />
    )}
</div>
```

<u>**logical &&**</u>

```javascript
<div>
    {isLoggedIn && <AdminPanel />}
</div>
```

rendering lists

```javascript

const products = [
    {title: 'Cabbage', id: 1},
    {title: 'Garlic', id: 2}
];

const listItems = products.map(product => 
    <li key={product.id}> {/*each item in a list should have a unique key*/}
        {product.title}
    </li>
);

return (
    <ul>{listItems}</ul>
)
```

```javascript
import { useState } from 'react';

function MyButton() {
    const [something, setSomthing] = useState(initialValue)
}

export default function MyApp() {
    return (
        <div>
            <MyButton /> {/*has its own state*/}
            <MyButton />
        </div>
    )
```

```javascript
function MyButton({ count, onClick }) { {/*to pass props*/}
    return (
        <button onClick={onClick}> {/*this action will lift state up*/}
            Clicked {count} times
        </button>
    );
}
```

Any function starting with "use" is a Hook. 
## Sources

ES6 Overview
- [ES6 Syntax and Feature Overview](https://www.taniarascia.com/es6-syntax-and-feature-overview/)

React
- [React - Hello World](https://reactjs.org/docs/hello-world.html)
- [React - JSX](https://reactjs.org/docs/introducing-jsx.html)
- [React - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
- [React - Components & Props](https://reactjs.org/docs/components-and-props.html)
- [React - State & Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
- [React - Handling Events](https://reactjs.org/docs/handling-events.html)

Tailwind CSS
- [Utility First CSS](https://tailwindcss.com/docs/utility-first)
- [Tailwind in a few minutes](https://www.youtube.com/watch?v=pB1oed_10IA)

Next.js
- [Learn Next.js](https://nextjs.org/learn/basics/create-nextjs-app)
- [Why to use Next.js](https://www.youtube.com/watch?v=rtgbaKBhdkk)

Reading Questions
1. In the context of ES6 Syntax and Feature Overview, what are three key features introduced in ES6 that improve upon the previous version of JavaScript, and briefly explain their benefits?
> Introduction of `let` keyword wich allows for block-scoped variables which cannot be hoisted or redeclared. Expressions can be embedded in template literal strings. This is more intuitive and also makes the code easier to read. Arrow function expression syntax which functions as an anonymous function that cannot be called. It has a shorter syntax and also easier to read.
2. After reading “Tailwind in 15 minutes,” can you describe the purpose of utility classes in Tailwind CSS and provide an example of how to use them to style an HTML element?
> The utility classes can be combined to create a custom style element. Example: `class = p-6 max-w-wm mx-auto bg-white rounded-xl shadow-lg flex items-center w-[300px]`

3. Based on “Why to use Next.js,” explain the main advantages of using Next.js for web development, and provide a brief comparison between traditional client-side rendering and Next.js’s server-side rendering approach.
> The advantages include choice of either client or server-side rendering on per page basis, easier to maintain performance as the number of pages grow, preservation of react state, and debugging modal. Because React can only be rendered on the client side, the developer has to use a different framework to build the server application. With Next.js' hybrid rendering, you can do both build both the client and server in a single framework.