# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). 

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

Create an NFT preview card component

### The challenge

Your challenge is to build out this preview card component and get it looking as close to the design as possible. You can use any tools you like to help you complete the challenge. 

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

#Screenshot 

Final Solution Screenshot

![](https://github.com/atreska/nft-preview-card/blob/main/images/Screen%20Shot%202024-04-16%20at%208.41.17%20PM.png)


### Links

- Solution URL: [](https://github.com/atreska/nft-preview-card)
- Live Site URL: [](https://atreska.github.io/nft-preview-card/)

## My process

- Created the HTML markup.
- Styled the HTML with css.
- Used flexbox to position the elements.
- Used percentages instead of pixels for a responsive page.
- Created hover effects using positioning, ::before, and background.


### Built with

- HTML
- CSS
- Flexbox

### What I learned

I got stuck on the hover effect for the main image. I had never used postion, ::before, or background properties before. After doing a little research, I was able to achieve the effect of hoving over the main image and having the icon show over the anchor tags background color.

```html
 <a href="#" class="anchor">
          <img class="main-picture hover" src="./images/image-equilibrium.jpg"
            alt="NFT Equilibrium Colored Cube with description.">
        </a>
```
```css
.anchor {
    display: block;
    position: relative;
}

.anchor:hover::before {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background-color: hsla(178, 100%, 50%, 0.5);
    background-image: url(./images/icon-view.svg);
    background-repeat: no-repeat;
    background-position: center;
    border-radius: .5em;

}
```

### Continued development

In the future I will be working on better semantic HTML, responsive design, css grid, and react. 

## Author

- Github - [@atreska](https://github.com/atreska)
- Frontend Mentor - [@atreska](https://www.frontendmentor.io/profile/atreska)

