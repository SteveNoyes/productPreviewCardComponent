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

## Overview
  This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa)
### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Github](https://github.com/SteveNoyes/productPreviewCardComponent)
- Live Site URL: - [GitHub Pages](https://stevenoyes.github.io/productPreviewCardComponent/)

## My process

### Built with

- HTML5 with help from Emmet
- CSS 
- Flexbox
- Mobile-first workflow
- VSCode
- Google

### What I learned

vertical-align: middle; 
It took a long time to find out how to center text next
to text. 

```html
<div class="prices">
  <p>
    <span class="current-price">$149.99</span>
    <span class="old-price">$169.99</span>
  </p>
</div>
```
```css
.current-price {
  font-family: 'Fraunces', sans-serif;
  color: var(--primary-dark-cyan);
  font-size: 2.3rem;
  margin-right: 2rem;
  vertical-align: middle;
}
```

After setting up the container, it took some time to position them beside each other. Finally I used flex 1 for the two divs in the container.

```css
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 90%;
  margin: 2rem auto 0;
  background-color: var(--neutral-white);
  border-radius: 15px;
}
```
```css
.perfume-image {
  flex: 1;
  width: 100%;
  border-radius: 15px 15px 0 0;
}
.text-wrapper {
  flex: 1;
  margin: 2rem;
}
```

The color on hover for the 'add to cart' button looked different than the ones provided so I put the image on an html page and used a color picker app


```css
:root {
  --active-dark-cyan: 	hsl(156, 42%, 18%);
}
```
 
Changing image on media query

```html
  <img class="perfume-image"/>
```
```css
  .perfume-image {
    content:url('./img/image-product-desktop.jpg');
  }
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

### Useful resources

- [The Markdown Guide](https://www.markdownguide.org/) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

- [Reset CSS](https://meyerweb.com/eric/tools/css/reset/) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

- [Stick to Bottom](https://dev.to/nehalahmadkhan/how-to-make-footer-stick-to-bottom-of-web-page-3i14) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

- [Text & Word Spacing](https://www.w3schools.com/css/css_text_spacing.asp) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

- [Changing Image at Media Query](https://stackoverflow.com/questions/2182716/is-it-possible-to-set-the-equivalent-of-a-src-attribute-of-an-img-tag-in-css) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

## Author

- Website - [Steven Noyes](https://www.stevenmnoyes.com)
- Frontend Mentor - [@SteveNoyes](https://www.frontendmentor.io/profile/SteveNoyes)
- LinkedIn - [Steven Noyes](https://www.linkedin.com/in/steven-noyes/)
