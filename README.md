# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)

  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)

- [My process](#my-process)

  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

- [Author](#author)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./images/screenshot.png)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

In order to position the profile image correctly, I used transform: translate. However, this left the image element's space unaffected and still visible in the original position. So I had to add position: absolute / relative to take the image out of the document flow.

This [stackoverflow article](https://stackoverflow.com/questions/58177903/css-translate-creates-white-space-on-original-position) provided the solution I was looking for.

```css
.card {
  position: relative;
}
```

```css
.victor-img {
  width: 8em;
  border-radius: 50%;
  border: 5px solid var(--white);

  position: absolute;

  left: 25%;
  top: 17%;
}
```

```css
.transform {
  transform: translate(25%, 17%);
}
```

## Author

- Frontend Mentor - [@codercreative](https://www.frontendmentor.io/profile/codercreative)
