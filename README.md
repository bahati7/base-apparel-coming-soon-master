# Frontend Mentor - Base Apparel coming soon page solution

This is a solution to the [Base Apparel coming soon page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/base-apparel-coming-soon-page-5d46b47f8db8a7063f9331a0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)



## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - The `input` field is empty
  - The email address is not formatted correctly

### Screenshot

https://github.com/bahati7/base-apparel-coming-soon-master/blob/main/design/desktop-design.jpg

https://github.com/bahati7/base-apparel-coming-soon-master/blob/main/design/mobile-design.jpg

### Links

- Solution URL: https://www.frontendmentor.io/solutions/baseapparelcomingsoonmaster-B1d2c-4Bq

- Live Site URL: https://base-apparel-coming-soon-master7.netlify.app/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- Javascript



### What I learned

In this challenge I learned javascript email regex 

```javascript
function email_validation(e){
    e.preventDefault();

    var mailformat = /^\w+([\.\-]?\w+)*@\w+([\.\-]?\w+)*(\.\w{2,3})+$/;
    var email_name = document.getElementById('email');
    var email_value = document.getElementById('email').value;
    var email_length = email_value.length;

    if(!email_value.match(mailformat) || email_length === 0){
    document.getElementById('email_err').innerHTML = 'Please provide a valid email adress.';
    email_name.focus();
    document.getElementById('email_err').style.color = "hsl(354, 100%, 66%)";
    email_name.style.border="1px solid hsl(354, 100%, 66%)" ;
    
}
}
```





## Author

- Website - https://bahatiphilemon.netlify.app/
- Frontend Mentor - https://www.frontendmentor.io/profile/bahati7
- Twitter - https://twitter.com/PhilemonBahati



## Acknowledgments

Thank you to Frontend Mentor team - https://www.frontendmentor.io/