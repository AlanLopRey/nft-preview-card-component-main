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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

Desktop
![](/images/Desktop%20version%20Frontend%20Mentor%20NFT%20preview%20card%20component.png)

Mobile
![](/images/Mobile%20version%20Frontend%20Mentor%20NFT%20preview%20card%20component.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Responsive Web Design

### What I learned

This was pretty challenge due to the hover element that shows a cyan background transparent and a eye in the middle, the way i do it was incerting the color insde the div containing the image and incerting the img of the eye inside the color container, I chose to set the image from the CSS code to have more control of it, also i remember the propertie background-size and set to cover to make the image of the size of the imageContainer, background position for the eye

```html
<div class="imageContainer">
  <div class="colorContainer">
    <div class="eyeContainer"></div>
  </div>
</div>
```

```css
.imageContainer {
  background-image: url(../images/image-equilibrium.jpg);
  background-size: cover; /*new property used*/
  width: 280px;
  height: 280px;
  margin-bottom: 28px;
  border-radius: 8px;
}

.colorContainer {
  background-color: var(--Cyan_hover);
  width: 100%;
  height: 100%;
  border-radius: 8px;
  opacity: 0;
}

.eyeContainer {
  background-image: url(../images/icon-view.svg);
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-position: center; /*NEW CODE USE*/
}

.colorContainer:hover {
  opacity: 1;
  cursor: pointer;
  /*Now i know how to produce this kind of hover*/
}
```

### Continued development

more use of all Flexbox propierties, readmore the documentation of CSS and try to use Grid in next challenge, also try to get better at english for the MarkDown lol

## Author

- Frontend Mentor - [@AlanLopRey](https://www.frontendmentor.io/profile/AlanLopRey)
