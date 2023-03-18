## Local Storage and How to Use it on Websites

**Notes**

HTTP is stateless

Local storage stores a key on the user's computer and accesses it when the user returns. It only stores string values. `JSON.stringify(object)` and `JSON.parse()` come in handy when objects are stored. Looks like `JSON.parse()` loops through the object and returns the values.

Cookies are outdated and some users will reject cookies

To use local storage in HTML5 supported browsers, you modify the `localStorage` object in JavaScript via setItem() or getItem() method

**localStorage methods()**

`localStorage.setItem('key','value');`

`localStorage.getItem('key') returns the 'value'.`

`localStorage.removeItem('key')` returns `null`

`sessionStorage`works similarly but only maintains data while the browser window stays open

`if(localStorage && localStorage.getItem``('thewholefrigginworld')){` first statement ask whether localStorage is supported, second statement checks if key called 'thewholefrigginworld' exists
  `render(JSON.parse(localStorage.getItem``('thewholefrigginworld')));` this statement executes if above is true, step one is getItem, step two is parse, step three is render
`} else {` if not true, below line executes (call to to GEO API) not quite sure what it truly means though
  `$('#list').html('`

  `YUI().use('node', function(Y) {`
  `if(('localStorage' in window) && window['localStorage'] !== null){` these statements look almost identical?
    `var key = 'lastyahoofirehose';`

   ` localStorage.setItem(key,Y.one('form').get('innerHTML'));`

  `if(key in localStorage){`
      `Y.one('#mainform').set('innerHTML',localStorage.getItem(key));`
      `Y.one('#hd').append('`


**Q&A**

1. Why would a developer use local storage for a web application? So they can persist data without a server, and also so they don't use up all their quota?

2. What information should not be stored in local storage?

3. Local storage can store what type of data? strings
How would you convert it to that type before storing

## Bookmark
[The Past, Present, and Future of Local Storage for Web Applications](http://diveinto.html5doctor.com/storage.html)

### Things I want to know

Link to github