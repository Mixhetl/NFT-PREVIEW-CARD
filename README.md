# Frontend Mentor - QR code component solution

This is a solution to the [NFT preview card component](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U/hub/nft-preview-card-component-gAOXqx56-). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot - NFT Preview Card](design/Screenshot%20Frontend%20Mentor%20NFT%20preview%20card%20component.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/Mixhetl/NFT-PREVIEW-CARD)
- Live Site URL: [Add live site URL here](https://mixhetl.github.io/NFT-PREVIEW-CARD/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned

This was my first practice, and I learned to use HTML for the first time without seeing any tutorial about it. I also ventured to use CSS styles with my own criteria. It gave me confidence to keep trying other exercises. I liked

```html
<body>
  <div class="shadow">
    <div class="container">
      <figure>
        <img src="images/image-equilibrium.jpg" alt="equilibrium" />
        <div class="cape">
          <img src="images/icon-view.svg" alt="" />
        </div>
      </figure>
      <div>
        <a href="#">Equilibrium #3429</a>
        <p>
          <span class="iridicent"
            >Our Equilibrium collection promotes balance and calm.</span
          >
        </p>
      </div>
      <div class="content">
        <div class="display">
          <img src="images/icon-ethereum.svg" alt="" />
          <p><span class="--iridicent">0.041 ETH</span></p>
        </div>
        <div class="display">
          <img src="images/icon-clock.svg" alt="" />
          <p><span class="iridicent">3 days left</span></p>
        </div>
      </div>
      <div class="--content">
        <img src="images/image-avatar.png" alt="avatar" />
        <p>
          <span class="iridicent">Creation of</span><a href=""> Jules Wyvern</a>
        </p>
      </div>
    </div>
  </div>
</body>
```

```css
:root {
  /**Primary Colors**/
  --soft-blue: hsl(215, 51%, 70%);
  --cyan: hsl(178, 100%, 50%);

  /**Neutral Colors**/
  --main-bg: hsl(217, 54%, 11%);
  --card-bg: hsl(216, 50%, 16%);
  --inline: hsl(210, 44%, 22%);
  --white: hsl(0, 0%, 100%);

  /* Font Sizes */
  --fs-400: 1.125rem;
  --fs-300: 1rem;
}

/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin */
body,
h1,
h2,
h3,
h4,
p,
figure {
  margin: 0;
}

/* Remove list styles on ul, ol elements with a list role, which suggests default styling will be removed */
ul[role="list"],
ol[role="list"] {
  list-style: none;
}

/* Set core root defaults */
html:focus-within {
  scroll-behavior: smooth;
}

/* Set core body defaults */
body {
  height: 100%;
  text-rendering: optimizeSpeed;
  line-height: 1.5;
  background-color: var(--card-bg);
  display: grid;
  justify-items: center;
  align-items: center;
  grid-gap: 10px 1rem;
  color: var(--white);
  font-family: "Outfit", sans-serif;
  padding: 2rem;
}

/* Inherit fonts for inputs and buttons */
input,
button,
textarea,
select {
  font: inherit;
}

div a {
  font-size: var(--fs-400);
  text-decoration: none;
  color: var(--white);
}

div a:hover {
  color: var(--cyan);
  backdrop-filter: blur(20px);
}

/* Remove all animations, transitions and smooth scroll for people that prefer not to see them */
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
    scroll-behavior: auto;
  }

  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}

/* Custom styles */
.container {
  width: 320px;
  height: 540px;
  border-radius: 10px;
  padding: 1.5rem;
  margin: 1rem;
  background-color: var(--inline);
}

.container:first-child img {
  margin-bottom: 10px;
}

.shadow {
  width: 350px;
  padding: 0;
  background-color: var(--main-bg);
  border-radius: 10px;
  margin: 10px;
}

.attribution {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 2rem;
}

figure {
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 65%;
}

figure img {
  width: 100%;
  margin: 0 auto;
  border-radius: 10px;
  transition: all 500ms ease-out;
}

.cape {
  width: 100%;
  height: 85%;
  border-radius: 10px;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  background-color: hsla(178, 100%, 50%, 0.4);
  transition: all 500ms ease-out;
  opacity: 0;
  visibility: hidden;
}

figure:hover > .cape {
  opacity: 1;
  visibility: visible;
  cursor: pointer;
}

.cape img {
  width: 40%;
}

.iridicent {
  color: var(--soft-blue);
}

.--iridicent {
  color: var(--cyan);
  font-weight: bold;
  font-size: var(--fs-300);
}

.content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 10px;
  margin-top: 10px;
  border-bottom: 1px solid hsl(215, 51%, 70%);
}

.--content {
  display: flex;
  align-items: center;
  justify-content: left;
  margin-top: 10px;
}

.--content img {
  width: 40px;
  margin-right: 10px;
  margin-left: 0;
}

.display {
  display: flex;
}

.display p,
img {
  margin: 5px;
}
```

### Continued development

Get better at using HTML. I will start this week to learn BEM methodology.

## Author

- Frontend Mentor - [@Mixhetl](https://www.frontendmentor.io/profile/Mixhetl)
- Twitter - [@XxmalkyelxX](https://twitter.com/XxmalkyelxX)

## Acknowledgments

Nothing right now :(
