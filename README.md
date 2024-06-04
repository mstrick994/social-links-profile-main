# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover and focus states for all interactive elements on the page

### Screenshot

![Screenshot of the solution](./Screenshot/Social-links-screenshot.png)

### Links

- Solution URL: [GitHub Repository](https://your-solution-url.com)
- Live Site URL: [Live Demo](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Animations
- Mobile-first workflow
- Vanilla JavaScript

### What I learned

During this project, I focused on implementing CSS animations and transitions, as well as JavaScript to enhance the user experience. Below are some key code snippets and explanations:

#### CSS Transitions and Animations

The card fades in from the bottom to the top using the `fadeInUp` keyframes animation:

```css
.body {
  background-color: var(--clr-secondary-drkgry);
  display: flex;
  flex-direction: column;
  gap: 1rem;
  border-radius: 0.5rem;
  padding: 1rem;
  transform: translateY(100%);
  animation: fadeInUp 2s ease-in-out forwards;
}

@keyframes fadeInUp {
  from {
    transform: translateY(50px); /* Start 50px below */
    opacity: 0;
  }
  to {
    transform: translateY(0); /* End at the original position */
    opacity: 1;
  }
}
```

#### JavaScript for Initial Fade-In

The following JavaScript code ensures that the fade-in animation is applied when the content loads:

```javascript
document.addEventListener('DOMContentLoaded', function() {
  const card = document.getElementById('card');
  card.classList.add('fade-in');
});
```

This script listens for the DOMContentLoaded event and then adds the `fade-in` class to the card element, triggering the CSS animation.

### Continued development

In future projects, I plan to:

- Further explore advanced CSS animations and transitions.
- Improve JavaScript skills for more complex interactive elements.
- Optimize performance for animations on different devices.

### Useful resources

- [CSS Tricks: Using CSS Transitions](https://css-tricks.com/almanac/properties/t/transition/) - This resource helped me understand the basics of CSS transitions and how to apply them effectively.
- [MDN Web Docs: Using CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations) - A great article on creating and using CSS animations.
- [JavaScript Event Listeners](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener) - This MDN article helped me implement the DOMContentLoaded event for my JavaScript code.

## Author

- Frontend Mentor - [@CodeWalker](https://www.frontendmentor.io/profile/Codewalker)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

