# Class 01
Date: *02/04/2023*

## Getting Started

*[Source](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Installing_basic_software)*

Tools in the professional toolkit include; 
- a computer
- a text editor
- a web browser
- a graphics editor
- a VCS
- an FTP (file transfer protocol)
- an automation system
- libraries, frameworks, etc to speed up writing common functionality


### How the Web Works

*[Source](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)*

- DNS (Domain Name System) is like an 'address book for websites' aka IP address e.g., 63.245.215.20
- TCP/IP defines how data traverses the net
- HTTP defines how clients and servers communicate
- Component files consist of code files and assets

### Order in which component files are parsed
1. HTML file
2. *links*
3. *scripts*
4. in-memory DOM, in-memory CCSOM, parsed JavaScript?

### Website Design and Process

Great reference for later *see* *[here](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like)*

### Javascript Basics
 
*[Source](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)*

With JavaScript you can write games, add prompts, click buttons, enter form data, add animations, dynamic styling etc

Invented by: *[Brandon Eich](https://en.wikipedia.org/wiki/Brendan_Eich)*

Helpful tools that unlock extra functionality within JavaScript with minimum effort include;

- Built-in browser Application Programming Interfaces (APIs)
- Third-party APIs that allows you to pull data from sources like Twitter or Facebook
- Third-party frameworks and libraries

### Q&A
1. Compose a short poem describing how HTTP sends data between computers. Client sends a HTTP request to the server and the server returns a HTTP response to the client.  
2. Describe how HTML, CSS and JS files are parsed in the browser. I don't know the answer to this but will try to remember to research later.
3. How can you find images to add to a Website? 
--> search Google Images
--> filter for Creative Commons License
--> copy image address or download to local machine and reference locally
4. How do you create a String vs a Number in JavaScript? Strings are enclosed within quotes and a Number is not enclosed in quotes.
5. What is a Variable and why are they important? a variable is a container that stores data that *may* change. Variable data types include String, Number, Boolean, Array, and Object. Variables are important because they allow dynamic programming in JavaScript.

Comments in Javascript are wrapped within /* & */ or prefix // if it is a single line

## Introduction to HTML



HTML comments are enclosed within &lt!-- --&gt

### Q&A
1. What is an HTML attribute? They are extra information that describe the tags in more detail.
2. Describe the Anatomy of an HTML element. It includes an opening tag, closing tag, and content in between.
3. What is the Difference between *article* and *section* element tags? These are semantic tags. Article element represents an article or body of work. [Source.](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article) A section represents a generic section of a document and should always have titles. [Source.](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section)
4. What Elements does a typical website include? *html*, *header*, *head*, *body*, *main*, *footer*, etc.
5. How does metadata influence SEO? This is the paragraph or page description that appears when you do a search
6. How is the *meta* HTML tab used when specifying metadata? charset helps the browser know which character set is used

## Miscellaneous

### More Q&As

### How to start to design a Website
1. What is the first step to designing a Website? Planning or project ideation
2. What is the most important question to answer when designing a Website? Purpose

### Semantics
1. Why should you use an *h1* element over a *span* element to display a top level heading? span is like a div or all-purpose element container whereas h1 is a semantic element that serves an actual purpose of a top-level heading
2. What are the benefits of using semantic tags in our HTML? improved SEO, assists screen readers, code readability, etc.

### What is JavaScript?
1. Describe 2 things that *require* JavaScript in the Browser? my brain is maxxed, will read and answer later
2. How can you add JavaScript to an HTML document? same as above

### Things I want to know more about

- Graphics editor such as GIMP and Figma
- Automation systems such as Webpack, Grunt, and Gulp
- Examples of comprehensive database-driven apps built in JavaScript
- [APIs](https://developer.mozilla.org/en-US/docs/Glossary/API)
- Working with Amazon and eBay APIs
- [Script loading strategies](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript#script_loading_strategies)
- [DOM API](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- When navigating back and forth between pages, how does the browser know which section I last left off?
- [Guide to Semicolons in JavaScript](https://www.codecademy.com/resources/blog/your-guide-to-semicolons-in-javascript/)
- character references