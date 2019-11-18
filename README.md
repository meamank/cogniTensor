# CogniTensor 

## 1.What is the difference between the fixed, absolute, relative and sticky value of position property? Provide the benefits of one over the other. Also, provide some use cases.

## 2. What is the difference between flex, float, and grid? What are the use cases for each? What is your preferred value and why is that so?

## 3. How do you optimize websites? Please provide all techniques or methods you have used in optimization?


## 4. Advantages and disadvantages of JS and CSS animation. What is your preferred way? Provide justification for that as well.


## 5. What are your preferred frontend libraries or technologies? Provide pros and cons of them which you have faced. If you can provide for what purpose you have used them then please do so.

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



## 8. Create a section displaying user profile. It should display user info and also allow user to upload a picture.
