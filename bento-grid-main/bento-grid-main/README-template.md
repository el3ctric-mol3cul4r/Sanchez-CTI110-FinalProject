# CTI-110 Final Project - Bento Grid by Charlie Sanchez

## Table of contents

- [CTI-110 Final Project - Bento Grid by Charlie Sanchez](#cti-110-final-project---bento-grid-by-first-name-last-name)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Useful resources](#useful-resources)
  - [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size

### Screenshot

![](./cti_screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox or other browser to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

### Links

- Repository URL: [Add repository URL here](https://github.com/el3ctric-mol3cul4r/Sanchez-CTI110-FinalProject.git)
- Live Site URL: [Add live site URL here](https://el3ctric-mol3cul4r.github.io/Sanchez-CTI110-FinalProject/)

## My process

### Built with

FILL THIS OUT WITH WHAT YOU USED!!! - Mr. Gardner

- CSS custom properties
- CSS Grid
- A tiny tiny bit of flexbox

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

I didn't really learn much surrounding html. However, I learned tons about CSS. For example, I learned how to use CSS grids. I did brute-force most of the span ranges, but they work on the desktop version, which is good enough.

```css
.item1 {
    grid-row: span 3 / span 5;
    background-color: hsl(31, 66%, 93%);
    font-size: 30px;
    margin-top: 20px;
    margin-left: 90px;
    margin-bottom:-20px;
    padding-top: 70px;
    padding-right: 30px;
    text-align: center;
    border-radius: 10px;
}
```
Also, I learned how to use media queries to make my website mobile compatible. The solution I deployed was a flexbox inside of the media query. This allowed me to organize the grid into one scrollable column, and I was able to override any grid rules.

```css
@media (max-width: 768px) {

  .parent {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }

  .parent > * {
    grid-column: auto !important;
    grid-row: auto !important;
    width: 100%;
  }
}
```


### Continued development

I definitely need to review whatever the heck mobile compatibility was. I also want to learn more about flexbox, and I'd like to use that next time instead of fixed grids. And next time, I'll definitely create the mobile layout first, and then change it for desktop, not vice versa. 

### Useful resources

- [CSS Grid Layout Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) - This REALLY helped with figuring out the grid layout of the bento website. It's insanely detailed while still staying concise and clear.
- [CSS Rounded Corners](https://www.w3schools.com/css/css3_borders.asp) - This helped me know how to use the border-radius property, because the parameters were initially confusing to me.
- [Improving Mobile First Design with CSS Grid](https://blog.pixelfreestudio.com/how-to-improve-mobile-first-design-with-css-grid/#aioseo-enhancing-mobile-first-design-with-css-grid) - This was a great resource for learning about media queries. Optimizing or at least making the mobile version legible was the worst part of this project. However, this simplified the solution for me.

## Author

- Website - [Charlie Sanchez](https://el3ctric-mol3cul4r.github.io/Sanchez-CTI110-FinalProject/)

