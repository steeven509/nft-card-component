# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

-   [Overview](#overview)
    -   [Links](#links)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)
-   [Author](#author)

## Overview

![](./images/desktop-design.jpg)

### Links

-   Solution URL: [github code source](https://your-solution-url.com)
-   Live Site URL: [NFT card component website](https://your-live-site-url.com)

## My process

### Built with

-   Semantic HTML5 markup
-   CSS custom properties
-   Flexbox
-   CSS Grid
-   Mobile-first workflow

### What I learned

I had already done this challenge but there was a lot of feedback, in the hovereffect of the bottom image it protrudes a few millimeters compared to the size of the image it was the first challenge now I'm fixing this problem , so I create a ::before in this I add the image with the content property: rather than going through the html, it's the logo of the eyes that is used for hovering in the ::before and then there is still a little excess but i just reduce the height: 98% by 2% and everything is fine now.

```css
.card .card__img-container::before {
    content: url("../images/icon-view.svg");
    position: absolute;
    width: 100%;
    height: 98%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 255, 247, 0.8);
    border-radius: 0.5rem;
    transition: 0.3s;
    cursor: pointer;
    opacity: 0;
}
.card .card__img-container:hover::before {
    opacity: 1;
}
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

## Author

-   Frontend Mentor - [@steeven509](https://www.frontendmentor.io/profile/steeven509)
