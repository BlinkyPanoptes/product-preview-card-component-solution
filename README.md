# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

#### Desktop View
![](./Desktop%20View.png)

#### Mobile View
![](./Mobile%20View.png)

### Links

- Solution URL: [Frontend Mentor Solution Page](https://www.frontendmentor.io/solutions/product-preview-card-component-using-flexbox-and-picture-tag-u9W6qGZ9zH)
- Live Site URL: [GitHub Pages Live Demo](https://blinkypanoptes.github.io/product-preview-card-component-solution/)

## My process

### Built with

- Semantic HTML5 markup
- CSS Custom Properties (Variables)
- Flexbox
- Mobile-first workflow
- `<picture>` element for responsive asset swapping

### What I learned

During this project, I reinforced my understanding of writing adaptive mobile-first code layouts. I learned how to use the standard HTML `<picture>` wrapper to dynamically swap out high-resolution background imagery between smartphone and desktop screen views without breaking accessibility or wasting bandwidth.

```html
<header class="product-card-img_container">
  <picture>
    <source media="(min-width: 1440px)" srcset="images/image-product-desktop.jpg">
    <img src="images/image-product-mobile.jpg" alt="Square glass bottle of Gabrielle Chanel perfume resting on a neutral surface">
  </picture>
</header>

I also deepened my mastery of CSS Flexbox logic when handling full-width structural ratios and vertically aligning components cleanly inside viewports.

```CSS
@media screen and (min-width: 1440px) { 
    .product-card {
        flex-direction: row;      
        max-width: 600px;
        width: 100%;
    }

    header,
    .product-card-content {
        flex: 1;
    }
}