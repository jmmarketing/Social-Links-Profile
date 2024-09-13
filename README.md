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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

Build out this social links profile and get it looking as close to the design as possible.

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./assets/images/social-links-screenshot.png)

### Links

- Solution URL: [GitHub](https://github.com/jmmarketing/Social-Links-Profile-FEM)
- Live Site URL: [Live](https://jmmarketing.github.io/Social-Links-Profile-FEM/)

## My process

Nothing crazy here. Started with HTML and pre-planning some basic class BEM conventiions.

Used Figma file to get the sizing requirements for fonts, spacing, etc..

Built out bare-bones SCSS file structure (mixins, base, typography, components).

### Built with

- Semantic HTML5 markup
- SCSS custom properties
- Flexbox
- No, Zero, Zip, Nada JavaScript needed.

### What I learned

Using this as a way to hone in and polish my front end skills. CSS/SCSS has grown over the last half decade, so being able to fluently add it to my skillset is what my focus was.

Below is the whole card component.

```html
<div class="card">
  <div class="card__avatar"></div>
  <div class="card__information-block">
    <h2 class="heading-secondary">Jessica Randall</h2>
    <p class="card__location">London, United Kingdon</p>
  </div>
  <p class="card__description">"Front-end developer and avid reader."</p>
  <ul class="card__link-container">
    <li class="card__link">GitHub</li>
    <li class="card__link">Frontend Mentor</li>
    <li class="card__link">LinkedIn</li>
    <li class="card__link">Twitter</li>
    <li class="card__link">Instagram</li>
  </ul>
</div>
```

```css
.card {
  background: #1f1f1f;
  border-radius: 12px;

  max-width: 384px;
  padding: 40px;

  display: flex;
  flex-direction: column;
  flex: 1 0 0;
  align-items: center;
  gap: 24px;

  text-align: center;

  @include respond(tablet) {
    max-width: 456px;
  }

  &__avatar {
    height: 88px;
    width: 88px;
    border-radius: 999px;
    background: url(../assets/images/avatar-jessica.jpeg) lightgray 50% / cover
      no-repeat;
  }

  &__information-block {
  }

  &__location {
    color: #c4f82a;
    font-size: 1.4rem;
    font-weight: 700;
    line-height: 150%;
  }

  &__description {
    font-size: 1.4rem;
    font-weight: 300;
    font-style: normal;
    line-height: 150%;
  }

  &__link-container {
    text-decoration: none;
    list-style: none;
    width: 100%;
  }

  &__link {
    padding: 12px;
    // width: 100%;

    font-size: 1.4rem;
    font-weight: 700;

    background: #333;
    border-radius: 8px;

    &:not(:last-child) {
      margin-bottom: 16px;
    }

    &:active,
    &:hover {
      background: #c4f82a;
      color: #000;
    }
  }
}
```

### Continued development

Again, this is to continue developming my CSS/SCSS skills, outside of the standard padding/margin/align/etc.. While I enjoy Javascript, I recognize there is a lot of over-engineering UI, while there are perfectly acceptable (less resources needed) ways of using psuedo-classes, functions, and mixins to get the same result.

### Useful resources

- [SCSS Resource](https://sass-lang.com/guide/) - Good old documentation.

## Author

- Website - [Jeffrey McLean](https://jeffreymclean.com)
- Frontend Mentor - [@jmmarketing](https://www.frontendmentor.io/profile/jmmarketing)
- Twitter - [@jeffe_mclean](https://www.twitter.com/jeffe_mclean)
