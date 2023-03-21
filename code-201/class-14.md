## CSS Transforms
[Source](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

Notes

`transform` property has two settings, 2D or 3D. 

`div {`

  `-webkit-transform: scale(1.5);`

    `-moz-transform: scale(1.5);`

       `-o-transform: scale(1.5);`

          `transform: scale(1.5);`

`}`

webkit, moz, o are all vendors

the last un-prefixed declaration overwrites the prefixed versions

2D works on x and y axis
3D works on x, y, and z axis (length, width, depth)

transform properties
* rotate (how many degrees from 0 to 360), positive value rotates clockwise, default point of rotation is center of element 50% 50%
* scale (appeared size of element), default scale is 1, values between .01 - .99 is smaller, and values higher than 1 amake the element appear larger, use `scale(x,y)` if you want to scale each axis a different value and do it in one line
* scaleX changes the scale of the width
* scaleY changes the scale of the height
* translate works like relative positioning, uses any general length measurement such as pixels or percentages, positive values push an element down and to the right of its default position and negative pushes it up and left
* skew distorts the elements, uses degrees

if you need multiple transformations, do it on one line without the use of commas other CSS rules will cascade and overwrite the previous declaration


**Q&A**
1. What does a CSS transform allow the developer to do to an element? apply 2D or 3D animation
2. Provide an example of a transform and how you could see that being used on a website.

`.box-3 {`

  `transform: scale(.5, 1.15);`

`}`

this could be used to implement Zeegi's spinning card idea

## CSS Transitions & Animations
[Source](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

Notes

Transitions are applied to pseudo-classes
`:hover`
`:focus`
`:active`
`:target`

transition-property
transition-duration
transition-timing-function
transition-delay

**Q&A**
1. What does a CSS transition allow the developer to do to an element? apply transitions and animations to elements based on user behavior such as hover without javascript or the outdated Flash
2. How does a CSS animation differ from a CSS transition? animations have multiple states, and transition is single state changes

## 8 simple CSS3 transitions that will wow your users
[Source](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

Notes

**Q&A**
1. What are some benefits to using CSS transitions on websites? they're easy to implement, increase engagement, and ultimately increase conversions = $$$
2. How this topic fit in with your long-term goals? I think CSS animations are super cool. I had no idea that this was a thing.I can't wait to play around with this some more and create my own animations, then add them to my portfolio. 


### Bookmark/Skim
[Pure CSS Bounce Animation](https://codepen.io/dp_lewis/pen/QWMxRR)

[6 Buttons animated](https://codepen.io/retyui/pen/ByoaXV)

[CSS3 Animations: Keyframes](https://codepen.io/akshaychauhan/pen/dyBqVo)

[404](https://codepen.io/kieranfivestars/pen/MYdQxX)

### Things I want to learn more about
- transform matrix

