# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](<./design/screenshot.png>)

### Links

- Solution URL: (https://your-solution-url.com)
- Live Site URL: (https://your-live-site-url.com)

## My process

I first started to learn HTML and CSS fundamentals in Spring of 2021. Since then, I've shifted a large part of my focus to JavaScript and programming concepts. Working on this project was a great interactive refresher for all of the various CSS properties and how they come together to design a single element on the web page. The two areas that I feel I grew the most in my understanding was in custom properties and alignment with flex and grid.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

Defining the Grid:
```html
  <main class="testimonial-grid">
    <article class="testimonial flow ">
    </article>
    <article class="testimonial flow ">
    </article>
    <article class="testimonial flow ">
    </article>
    <article class="testimonial flow ">
    </article>
    <article class="testimonial flow ">
    </article>
  </main>
```
```css
.testimonial-grid {
  display: grid;
  gap: 1.5rem;
  grid-auto-columns: 1fr;
  grid-template-areas:
    'one'
    'two'
    'three'
    'four'
    'five';

  padding-block: 2rem;
  width: min(95%, 70rem);
  margin-inline: auto;
}
```

Defining where Grid components start:
```css
.testimonial:nth-child(1) {
  grid-area: one;
}
.testimonial:nth-child(2) {
  grid-area: two;
}
.testimonial:nth-child(3) {
  grid-area: three;
}
.testimonial:nth-child(4) {
  grid-area: four;
}
.testimonial:nth-child(5) {
  grid-area: five;
}
```


### Useful resources

- [MDN Web Docs - Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/grid) - MDN Web Docs is always my go to resource to look up and review web development fundamentals in HTML, CSS, and vanilla JavaScript.
- ["Learn CSS Grid the easy way" by Kevin Powell](https://youtu.be/rg7Fvvl3taU?si=TGpfgZB2JMi9Zlkt) - This video tutorial helped guide me through the process of completing this component. It was useful because I only retained about 70% of the fundamentals of HTML and CSS from my other independent courses completed in early 2021.

## Author

- Website - [Jacob W. Warner](https://www.jacobwwarner.com)
- Frontend Mentor - [@jacobwwarner](https://www.frontendmentor.io/profile/jacobwwarner)
- LinkedIn - [@jacobwwarner](https://www.linkedin.com/in/jacobwarner/)
- Twitter - [@jacobwwarner](https://www.twitter.com/jacobwwarner)

## Acknowledgments

"Learn CSS Grid the easy way" by Kevin Powell
(https://youtu.be/rg7Fvvl3taU?si=TGpfgZB2JMi9Zlkt)
