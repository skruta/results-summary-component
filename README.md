# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
    - [Desktop](#desktop)
    - [Mobile](#mobile)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout of UI on desktop and mobile device
- See hover and active state for button

### Screenshot

#### Desktop

![](/design/desktop-solution.png)

#### Mobile

![](/design/mobile-solution.png)

### Links

- Solution [URL]([https://your-solution-url.com](https://github.com/skruta/results-summary-component))
- Live Site [URL](https://results-summary-component-7awwdirug-skruta.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- SASS
- Mixins
- Functions
- Variable Fonts

### What I learned

I learned how to use Variable Fonts and also add fallback static fonts for older browsers. You can see my approach bellow:

```scss
// Static fonts for older browsers
@font-face {
  font-family: 'Hanken Grotesk';
  src: url('/assets/fonts/static/HankenGrotesk-ExtraBold.ttf') format('woff2');
  font-weight: 800;
}

@font-face {
  font-family: 'Hanken Grotesk';
  src: url('/assets/fonts/static/HankenGrotesk-Bold.ttf') format('woff2');
  font-weight: 700;
}

@font-face {
  font-family: 'Hanken Grotesk';
  src: url('/assets/fonts/static/HankenGrotesk-Medium.ttf') format('woff2');
  font-weight: 500;
}

// Added support for variable fonts, if variable fonts are not supported, static fonts above will be used.
@supports (font-variation-settings: normal) {
  @font-face {
    font-family: 'Hanken Grotesk VF';
    src: url('/assets/fonts/HankenGrotesk-VariableFont_wght.ttf') format('woff2-variations');
    font-weight: 100 1000;
  }
}
```

### Useful resources

- [This article](https://web.dev/variable-fonts/) helped me to set-up variable fonts.

## Author

- Frontend Mentor - [@skruta](https://www.frontendmentor.io/profile/skruta)
