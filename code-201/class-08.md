# Class 08
Date: 2/28/2023

## Reading
### Learn CSS - Flexbox
[Source](https://web.dev/learn/css/flexbox/)

- main axis follows flex direction
- single line by default but can span multiple lines as needed
Visual order does not have to match the DOM order
- set by the flex-direction property
- main and cross axis are perpendicular
- flex items move as a group on the main axis
items can be moved individually or as a group on the cross axis

CSS Property
display: flex; //returns a block-level box, with flex item children

Initial values; flex-direction: row, do not wrap, do not grow, line up at the start of the container

any reverse properties negatively affect accessibility

1. Flexbox is designed for one-dimensional content. Explain what this means. You can choose to flex dsplay your content in only one direction either vertically or horizontally 
2. Explain the difference between the main axis and cross axis. items move as a group on the main, and items can be moved individually or as a group on the cross axis
3. How can using certain properties of flexbox negatively impact accessibility? row and column-reverse may not match the logical order in the DOM therefore can cause confusion to screen readers


### CSS Layout - Flexbox
[Source](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

Read up to “Flex-Flow Shorthand”

Steps to  
1. Determine parent element and change its display to "flex". parent element will become a flex container and the children become flex items
2.

horizontal axis moves left to right
vertical axis moves top to bottom
reverse does the opposite

display choices
1. flex
2. inline-flex

flex-flow replaces both flex-direction and flex wrap


1. What are some advantages of using flexbox over float? it's easier to work with
2. How does this topic connect with your long term goals? I'm not sure because I like doing things the hard way in the beginning at least

## Bookmark and Review
[Learn CSS - Layout](https://web.dev/learn/css/layout/)

### Things I want to know

