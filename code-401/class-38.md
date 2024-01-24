# Class 38: React 2

## Sources
- [React - Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)
- [React - List & Keys](https://reactjs.org/docs/lists-and-keys.html)
- [React - Forms](https://reactjs.org/docs/forms.html)
- [React - Lifting State](https://reactjs.org/docs/lifting-state-up.html)
- [React - Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

## Bookmark and Review
- [React - Comprehensive Guide](https://tylermcginnis.com/reactjs-tutorial-a-comprehensive-guide-to-building-apps-with-react/)
- [HeroIcons](https://heroicons.com/)

## Personal Bookmarks
- [JavaScript Overview](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Language_overview)

## Reading Questions

1. How does lifting state up in a React application help with managing data flow and what are the benefits of using this approach?
> If two components need to have the same data, then lifting that data/state to a common parent component will ensure consistent data across both components. The data/state will also be stored in a single location (single source of truth). 
2. Explain the concept of conditional rendering in React and provide an example of how to implement it in a component.
- [ChatGPT Prompt](https://chat.openai.com/c/f04d70db-4f2f-4f13-9ce9-ad1ba2a4b212)
> React will render/show content only if the conditional is True. You can implement it use if statements, ternaries, logical && operator, or switch (case) statements. 
>
```javascript
   {isAuthenticated ? <LogoutButton /> : <LoginButton />}
```
3. What are the main principles behind “Thinking in React” and how do they guide the process of designing and building a React application?
> The first principle is to break the UI into a component hierarchy, second is to build a static version, third is to identify the minimal but complete representation of UI state, next is to identify where state should live, and last to add inverse data flow. 