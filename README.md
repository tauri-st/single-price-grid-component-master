# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action (I am seeking feedback from the community regarding this requirement which is not evident to me from the Figma design comp.)

### Screenshot

![Desktop and Tablet Styles](/images/fem-grid-solution-screenshot.png)
![Mobile](/images/fem-grid-mobile-solution-screenshot.png)

### Links

- [Live site URL here](https://tauri-st.github.io/single-price-grid-component-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Clean grid layouts: Fixed sizing is not always desirable when it comes to responsive layouts, but this is a very specific and tightly knit grid so it's needed here. When I first tried to create the layout, I tried to create the sizing I saw within each div by setting fixed sizes for each div! This was messy and created grid overflow. Responses on the FEM Slack cleared up that I needed to set my fixed widths on the content wrappers instead. No fixed heights were necessary once everything else was arranged.

Pixels vs ems vs rems when it comes to accessability: The article I shared in resources about sizing units really got my wheels turning. For font sizes, I used to fix the pixels in the body then set an em in the HTML and refer to that in ems throughout the rest of the document. Now after learning that fixing the pixel size in the body disables a person from setting their own standard font size! So now I've switched to rems for fonts exclusively. I have also started using rems for horizontal margins (but not veritcal!) when between text in order to create better readability as the font size may be increased.

Buttons vs links: I had already read some things about using a hrefs vs buttons from [CSS Tricks](https://css-tricks.com/a-complete-guide-to-links-and-buttons/), but my button had nice margins and my link would disappear them! Well that's because anchor elements are inline, which of course inline elements wouldn't have manipulatable margins that makes sense! Thanks again to Grace for that observation.

Box shadow was a first for me, and fun to learn. Pretty explanatory once I got the right resource.

### Continued development

I challenged myself to use grid columns and rows for this challenge because I am fairly new to grid, but my peers on FEM and Kevin Powell have introduced grid-ares to me so I will be exploring that next.
This is my last layout built from scratch. I will be branching off into component libraries and specific Tailwind after this!

### Useful resources

- [Josh W Comeau on Pixels vs ems vs rems]((https://www.joshwcomeau.com/css/)surprising-truth-about-pixels-and-accessibility/) - This goes into depth into browser settings and font standards when discussing sizing units for accessability
- [MDN Docs Box Shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) - This was the best resource I could find that explains everything you need to know about box shadow.

## Author

- Website - [@tauri-st](https://github.com/tauri-st)
- Frontend Mentor - [@tauri-st](https://www.frontendmentor.io/profile/tauri-st)
- LinkedIn - [@tauri-stclaire](https://www.linkedin.com/in/tauri-stclaire/)
- My Blog on Code Newbie - [@taurist](https://community.codenewbie.org/taurist)

## Acknowledgments

Thank you @Vanza from the FEM Slack for introducing me to Josh W Comeau, he has a class on CSS for JS Developers and I'm VERY interested now after seeing how thorough he is!
Thank you @Grace from the FEM Slack for getting right to the core of my layout issues and providing helpful and direct feedback!

My Questions for the Community:
- The Project rerquirments state we should be able to "See a hover state on desktop for the Sign Up call-to-action?" but I don't see anything indicated like that in the Figma.
- The color displayed by Figma for the "why us" list as well as the Subscription "per month" is white, but they look to be a light grey? There is a drop shadow affect listed, is this an inset drop shadow?
- This is my last FEM hacking it on my own before using a component library! I'm going to explore Tailwind, and would appreciate any favorite resources :)