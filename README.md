# Frontend Mentor - Stats Preview Card Component Solution

This is a solution to the [Stats Preview Card Component Challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Links

- Solution URL: [Add solution URL here](https://github.com/NelPascual/order-summary-component)
- Live Site URL: [Add live site URL here](https://order-summary-card-nelpascual.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Among the things I was able to learn and practice in this project are:

- Use the grid lines to change the positioning of the columns.

- Overlay a layer over an image to apply a faded color to it.

Here are some examples:

```html
<main class="card-container container">
  <header class="header-image"></header>
  <section class="card-text-container"></section>
</main>
```
```css
.card-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 5rem;
}

.header-image {
  background-image: url(../img/image-header-desktop.jpg);
  grid-column: 2 / 3;
  height: auto;
}

.card-text-container {
  grid-column: 1 / 2;
  grid-row: 1 / 2;
}
```
```css
.header-image {
  background-image: url(../img/image-header-mobile.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  z-index: 1;
  height: 24.5rem;
}

.header-image::after {
  border-radius: 1.5rem 1.5rem 0 0;
  content:"";
  position:absolute;
  top:0;
  left:0;
  right: 0;
  bottom: 0;
  background-color: #aa5cdb79;
  z-index: 2;
}
```

### Continued development

This is my sixth project done on this platform, I had a problem with the image when displayed on screens between 740px and 940px, although I used;
- display: grid;
- grid-template-columns: repeat(2, 1fr);

The grid is not displayed proportionally, displaying the image with less width.

I will try to identify what I have done wrong so that this does not happen, any help will be appreciated.

## Acknowledgments

I thank Frontend Mentor for providing free resources to put into practice what I have learned, and above all a place to show them.
