# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). 

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

## My process
First I drew out the design on paper with all the information I needed (sizes, colors, divs, and margins). 
<br />Drawing the plan out allows me think less and not rely on the `style-guide`.

### Built with
- HTML and CSS

### What I learned

I learned that to add an svg icon into a button element, you just keep the button element open and insert the svg there.
<br/>[Taken from StackOverflow](https://stackoverflow.com/questions/34393465/add-svg-icon-into-button-with-css-html)

```html
<button type="button" name="purchase-button" class="purchase-button">
          <svg style="margin-right: 10px;" width="15" height="16" xmlns="http://www.w3.org/2000/svg">
            <path
              d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z"
              fill="#FFF" />
          </svg>
          <p class="body-text button-text">Add to Cart</p>
</button> <!-- This is what I mean -->
```


I never used CSS Media Queries before until this challege.
```css
@media screen and (max-width: 375px) {
  .product-container {
    flex-direction: column;
    max-width: 315px;
  }
/*...*/
```

Used the `<picture>` element to solve the problem of changing the image source based on the screen size.
```html
<picture>
          <source media="(max-width: 375px)" srcset="images/image-product-mobile.jpg">
          <img class="perfume-image" src="images/image-product-desktop.jpg" alt="Image of Gabrielle-Chanel-Paris perfume on cream 
                                                                                 background with leaves on bottom and top.">
</picture>
```

### Continued development

Using Flex layout more often because I'm bad at it.

## Author

- Frontend Mentor - [@abanZaman125](https://www.frontendmentor.io/profile/abanZaman125)
