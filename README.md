# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

[Desktop Solution](./screenshot-desktop.png)
[Mobile Solution](./screenshot-mobile.png)

### Links

- Solution URL: [Github Repo](https://github.com/jdnunez504/stats-preview-card)
- Live Site URL: [Github Page](https://jdnunez504.github.io/stats-preview-card/)

## My process

### Built with
- Semantic HTML5 markup
- Mobile-first workflow
- CSS custom properties
- Flexbox
- SCSS

### What I learned

- Mixins for responsive styles
- Creating color overlay for images
- Using images in an element vs in the background (this project uses the image in the background-image property)
- Practice with responsive styling between mobile and desktop
- Practice with mobile-first design
- Practice using flex-box
- Practice with using class components

To see how you can add code snippets, see below:

Div element for background image and overlay:
```html
<div class="main__overlay"></div>
```
Styling for image overlay:
```css
.main__overlay {
  height: auto;
  width: 100%;
  padding-bottom: 73.4%;
  overflow: hidden;
  position: relative;
  background-image: url(../../images/image-header-mobile.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  border-top-left-radius: 0.5rem;
  border-top-right-radius: 0.5rem;
}
.main__overlay::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: linear-gradient(to right, rgba(171, 92, 219, 0.4), rgba(171, 92, 219, 0.4));
  mix-blend-mode: color;
}
/* There is another overlay pseudo element added here but probably unecessary */
```

### Continued development

- Choosing breakpoints for devices
- CSS inheritance in responsive design
- BEM
- Limiting refactoring and planning ahead
- Using CSS Grid

### Useful resources

- [Code Pen](https://codepen.io) - Good for testing out different strategies (for image overlays in this project).
- [FrontEnd Resource](https://frontendresource.com/css-background-image-color/) - How to use color overlay with background images.
- [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size) - Reference for the background-size property.
- [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Good reference guide for flexbox.

## Author

- Github - [JD Nunez](https://github.com/jdnunez504)
- Frontend Mentor - [@jdnunez504](https://www.frontendmentor.io/profile/jdnunez504)