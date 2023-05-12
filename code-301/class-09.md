## Functional Programming Concepts

[Source](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming? According to the article on Medium.com, "Functional programming ... treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data".
2. What is a pure function and how do we know if something is a pure function? 
    1. it returns the same result if given the same arguments 
    2. it does not cause any observable side effects
3. What are the benefits of a pure function? it's stable, consistent, and predictable making is easier to test
4. What is immutability? means it does not change
5. What is Referential transparency? when a function consistently yields the same result for the same input, is is referentially transparent

pure functions + immutable data = referential integriy

## Node JS Tutorial for Beginners #6 - Modules and require()

[Source](https://www.youtube.com/watch?v=xHLd36QoS4k)

module.exports = functionName makes the functionName available outside of the module

1. What is a module? a js file that contains functions
2. What does the word ‘require’ do? it works like an import statement but is specific to node
3. How do we bring another module into the file the we are working in? use the require statement
4. What do we have to do to make a module available? module.export