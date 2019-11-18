# CogniTensor 

## 1.What is the difference between the fixed, absolute, relative and sticky value of position property? Provide the benefits of one over the other. Also, provide some use cases.
- "Position: static" is the default value that an element will have. This means if we don’t declare position for an element in CSS, it will automatically be set to static. For example, if we have multiple <div> elements one after the other, they will appear on the page directly below one another.
- "Position: relative" is similar to static in that relatively positioned elements will follow the normal flow of the webpage.The difference is that now if we have 2 div elements and 2nd one is set to relative then it will take the first one as base and then we can move 2nd div to relative of 1st one.
- "Position: absolute" This property won't follow the normal flow of the webpage and gets taken out of the flow.That means wen you take an element out of the normal flow by using position: absolute, it will look for an ancestor element that has its own position set. This is so the child knows what element it should position itself in relation to.
The main difference between relative and absolute positioning is that position: absolute will take a child element completely out of the normal flow of the document. And that child will be positioned in relation to the first parent element that has its own position set.
- "Position: fixed" - Position: fixed will take the element out of the normal flow, and also position it in the same place in the viewport (what’s visible on screen). This means that scrolling will not affect its position at all.
- "Position: Sticky" is similar to absolute but it is related to scrolling.Position: Sicky elements will initially behave like position: relative elements, but if we keep scrolling, they will get taken out of normal form and behave like fixed.This can be really useful if you want to stick an element that’s initially farther down the page to the top of the screen.

## 2. What is the difference between flex, float, and grid? What are the use cases for each? What is your preferred value and why is that so?
- Float:
    - This is a great way to set an image within a larger text article. It's not a very practical way to set up an entire web page layout because this layout method just doesn’t have as many built-in properties as Grid or Flex and cannot create complex layouts.
- Flex:
    - This is a great tool to let smaller UI elements look their best on any device.Unfortunately if you want to layout larger elements on the page,flex doesn't provide us with more control where we can change margins etc on maths level.
- Grid:
    - With grid, it’s easy to set up an entire layout design system for your website. Layouts may be nested within other layouts and grid also allows you to create extremely complex arrangements with precision. But Grid isn’t best for quick centering or placing an image within a larger text article.
    
- My go to method is still GRid because of the levell of complexity it can handlle and control it provides.
## 3. How do you optimize websites? Please provide all techniques or methods you have used in optimization?
- Firstly, We have to determine the objective of your website optimization. Different business types will have different objectives you will want to optimize for. For example, if you ran an eCommerce website, you’d want to figure out how to increase purchases. Hence, a website owner will conduct quantitative and qualitative research on key pages of the website that affect the ultimate goal of the site.
Now we can do optimizations based on different things.
~ IF images are taking too much time then optimize images using ShortPixel without losing qality.
~ JS/CSS minification is also an important aspect.
~ Cache management is also important in making a website load faster.
~ Using own css file is better rather than using premade ones likes BootStrap etc. They are heavy in size and not useful if you are not even using most of the things.

## 4. Advantages and disadvantages of JS and CSS animation. What is your preferred way? Provide justification for that as well.
- Advantages:
    - Animating with CSS is the simplest way to get something moving on screen
    - Useful for one-shot UI animations like toggling
    - Use JavaScript animations when you want to have advanced effects like bouncing, stop, pause, rewind, or slow down.
    - No libraries required in CSS
    - Use JavaScript when you need significant control over your animations.
    
- Disadvantages:
    - Can't do complex animations in CSS.
    - Creating animations with JavaScript is, by comparison, more complex than writing CSS transitions or animations.
    
  I prefer JS animation because of the control and power it provides you. You can take the fine grain control of the whole animations using JS.
## 5. What are your preferred frontend libraries or technologies? Provide pros and cons of them which you have faced. If you can provide for what purpose you have used them then please do so.
I have worked with very few frontend libraries or technologies such as React, jQuery, and SASS.
I prefer React.js.
Pros:
- Virtual DOM in ReactJS makes the user experience better and developer’s work faster
- Permission to reuse React components significantly saves time
- One-direction data flow in ReactJS provides a stable code
-  Developed by Facebook so large community support and constantly developing.
Cons:
- Poor documentation (ReactNative has better documentation in my opinion which kind of helps understanding react.js better)
- Due to this learning curve is huge.
- JSX’s complexity 


## 6. Create a dash ( - ) separated string ‘x-y-z-g-e-f-h-i-j’ from an object first. `first = { a: ['x', 'y', 'z'], b: ['g', 'e', 'f'], c: ['h', 'i', 'j'] };`. Explain your preferred method for manipulating or looping through arrays and objects.

```js
let finalResult = '';
var first = { a: ['x', 'y', 'z'], b: ['g', 'e', 'f'], c: ['h', 'i', 'j'] };
Object.keys(first).forEach((key,index) => {
    first[`${key}`].map(element => {
        finalResult === ''
            ? finalResult += element
            : finalResult += `-${element}`
    });
});

console.log(finalResult);
```

## 7. Write a piece of code for generating random color strings in javascript. Fill 12 square divs with these random colors (show generated color code on div) everytime a button is clicked. Also animate these divs (flipping the div or zooming in or out).

- You can check the implemention here : https://codepen.io/meamank/pen/oNNJwWo

## 8. Create a section displaying user profile. It should display user info and also allow user to upload a picture.
- You can find this solution in this repository under name " react-user-profile"
