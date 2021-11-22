# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Look that](./design/overview-my-project.jpg)

### Links

- Solution URL: (https://www.frontendmentor.io/solutions/nft-card-component-using-flexbox-and-grid-AHaHYqzyy)
- Live Site URL: (https://nostalgic-banach-6d0114.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox and Grid
- Sass
- Mobile-first workflow
### What I learned

How to use two img elementes inside a same div, center them and use :hover to make styles. 


```scss
.image-card {
  display: grid;
  max-width: 17.5rem;
  background-color: transparent;
  border-radius: 0.75rem;
  overflow: hidden;

  .art,
  .layer {
    grid-row: 1;
    grid-column: 1;
  }
  .art {
    position: relative;
    top: 0;
    left: 0;
    border-radius: 0.75rem;
    max-width: 100%;
  }
  .layer {
    opacity: 0;
    z-index: 1;
    align-self: center;
    justify-self: center;
  }

  &:hover {
    cursor: pointer;
    background-color: $cyan;
    .art {
      mix-blend-mode: multiply;
    }
    .layer {
      opacity: 1;
    }
  }
}

```

### Continued development
I really want to master the hover efect on the image, to create transitions with two o more elements (one above the other). That was to hard for me this time. 

### Useful resources

- [¿Cómo colocar dos elementos uno encima del otro, sin especificar una altura?](https://qastack.mx/programming/6780614/css-how-to-position-two-elements-on-top-of-each-other-without-specifying-a-hei) - This helped me to center tow elements on the image-card dive. I have some questions if that's the correct and optimized way. 

## Author

- Frontend Mentor - [@EdwinCacuango](https://www.frontendmentor.io/profile/EdwinCacuango)
- Twitter - [@edwincacuango](https://twitter.com/edwincacuango)

