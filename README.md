# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### Screenshot

![Challenge Solution](images/challenge-solution.png)

Above is a screenshot of my solution! The original goal of the desktop view of this challenge can be seen in `design/desktop-design.jpg`.

### Links

- Solution URL: [Repo Solution](https://github.com/realynnsio/challenge-qr-code-component)
- Live Site URL: [Live Site Solution](https://challenge-qr-code-component-rust.vercel.app/)

## My process

### Built with

- HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Though this challenge was a fairly simple one, I felt like it was very effective in refreshing my knowledge on HTML and CSS. Having the style guide was a great help in determining the colors, and to make it easier for myself I created custom properties for these colors in my code too!

```css
* {
      ...
      --slate-300: hsl(212, 45%, 89%);
      --slate-500: hsl(216, 15%, 48%);
      --slate-900: hsl(218, 44%, 22%);
    }
```
This way, I was able to reuse the colors above by simply calling `var(--slate-xxx)` instead of copying the `hsl` each time. Very convenient :D

The rest of the work was pretty straightforward. I created a `div` and gave it the `card` class and tweaked the card styling to match the reference picture provided, adding the contents along the way too.

My one hurdle with this challenge was remembering a way to vertically center the card, a common problem I always seem to forget the solution to... in the end I got a working solution by styling the `body` tag with an added `background` class as a flexbox like so:

```css
.background {
      background-color: var(--slate-300);
      height: 100vh;
      width: 100vw;
      display: flex;
      align-items: center;
      justify-content: center;
    }
```

I wonder if it's best practice to style the `body` tag though? If anyone has feedback on that, let me know!




## Author

- Website - [alma-nashrida](https://www.alma-nashrida.com)
- Frontend Mentor - [@realynnsio](https://www.frontendmentor.io/profile/realynnsio)
- LinkedIn - [Alma Putri Nashrida](https://www.linkedin.com/in/alma-putri-nashrida/)
