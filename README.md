# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:
- See hover and focus states for all interactive elements on the page

### Screenshot
<table>
  <tr>
    <th >Desktop (1440px)</th>
    <td><img  src="assets/screenshots/screenshot-desktop.png"></td>
  </tr>
  <tr>
    <th>Mobile (375px)</th>
    <td><img  src="assets/screenshots/screenshot-mobile.png"></td>
  </tr>
  <tr>
    <th>Hover</th>
    <td><img src="assets/screenshots/screenshot-hover.png"></td>
  </tr>
  <tr>
    <th>Focus</th>
    <td><img src="assets/screenshots/screenshot-focus.png"></td>
  </tr>
</table>

### Links

- Solution URL: [GitHub Repository](https://github.com/incmoga/social-links-profile-main)
- Live Site URL: [Live Demo](https://incmoga.github.io/social-links-profile-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Responsive design
- CSS transitions for hover effects
- Variable fonts
- clamp() function for fluid sizing
- Accessible focus states

### What I learned

1. **Responsive design with clamp()**:
```css
/* Fluid sizing without media queries */
.profile-card {
  width: clamp(20.4375rem, 87.2vw, 24rem);
  padding: clamp(1.5rem, 6.4vw, 2.5rem);
}
```

I successfully implemented responsive layouts using CSS clamp() function, allowing elements to scale smoothly between minimum, preferred, and maximum values without media queries.

2. **Avatar styling techniques**:
```css
/* Circular avatar with proper image scaling */
.profile-info__avatar {
  width: 88px;
  height: 88px;
  border-radius: 50%;
  overflow: hidden;
}
.profile-info__image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

3. **Advanced focus states**:
```css
/* Accessible focus states */
.social-links__item:focus-within {
  background-color: var(--colors-green);
}
.social-links__item:focus-within .social-links__link {
  color: var(--colors-grey-900);
}
```

Implemented accessible focus states using :focus-within pseudo-class that works for keyboard navigation while maintaining visual consistency with hover states.

### Continued development
In future projects, I want to explore in depth:
- Implement CSS Grid for complex layout scenarios
- Explore container queries for component-based responsiveness

## Author

- GitHub - [Maksim Semizhonov](https://github.com/incmoga)
- Frontend Mentor - [@incmoga](https://www.frontendmentor.io/profile/incmoga)
