# Frontend Mentor - Product Preview Card Component Solution
 
This is my solution to the Product Preview Card Component challenge on Frontend Mentor. The goal was to build a responsive product card as closely as possible to the provided mobile and desktop designs using HTML and CSS.
 
## Table of contents
 
- #overview
- #the-challenge
- #screenshot
- #links
- #my-process
- #built-with
- #what-i-learned
- #continued-development
- #useful-resources
- #ai-collaboration
- #author
 
## Overview
 
### The challenge
 
Users should be able to:
 
- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements
 
### Screenshot
 
screenshots\Screenshot 2026-10-01 155405.png
 
### Links
 
- Solution URL: [Add Frontend Mentor solution URL]
- Live Site URL:  https://qcyrus8j562z1111.github.io/product-preview-card-component/
 
## My process
 
I approached this challenge with a mobile-first workflow. I started by creating semantic HTML for the product card before moving into the CSS.
 
I established reusable color and typography variables, built the mobile layout first, and then added a breakpoint when the component had enough room to transition naturally into the desktop two-column layout.
 
I tested the component across a range of viewport widths rather than designing only for the 375px and 1440px reference sizes.
 
### Built with
 
- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Responsive images with the `<picture>` element
- CSS media queries
- Google Fonts
- Hover and `:focus-visible` interaction states
- Git and GitHub for version control
 
### What I learned
 
One of my biggest takeaways from this project was that the widths supplied by a design are reference sizes, not necessarily breakpoints. Instead of treating 375px as "mobile" and 1440px as "desktop," I tested the component across the full range of screen sizes and chose a 600px breakpoint based on when the layout itself had enough room to switch to two columns.
 
I also practiced responsive image handling with the `<picture>` element:
 
```html
<picture>
images/image-product-desktop.jpg
images/image-product-mobile.jpg
</picture>
```
 
Another useful technique was creating design tokens with CSS custom properties:
 
```css
:root {
--clr-green-500: hsl(158, 36%, 37%);
--clr-green-700: hsl(158, 42%, 18%);
--clr-black: hsl(212, 21%, 14%);
--clr-gray: hsl(228, 12%, 48%);
--clr-cream: hsl(30, 38%, 92%);
--clr-white: hsl(0, 0%, 100%);
 
--ff-montserrat: "Montserrat", sans-serif;
--ff-fraunces: "Fraunces", serif;
}
```
 
This made the stylesheet easier to read and gave me one place to manage the project's colors and typography.
 
I also learned more about accessible interaction states by giving the Add to Cart button separate mouse hover and keyboard focus styles:
 
```css
.product-button:hover {
background-color: var(--clr-green-700);
}
 
.product-button:focus-visible {
outline: 3px solid var(--clr-green-700);
outline-offset: 3px;
}
```
 
Finally, I got more practice using Git as part of the development process. I reviewed changes with `git diff`, created commits around meaningful project milestones, and even used Git to recover `index.html` after accidentally deleting it.
 
### Continued development
 
Going forward, I want to continue improving:
 
- Responsive layout design
- Translating static design references into CSS more efficiently
- Typography and visual design matching
- Accessible interaction states
- Choosing breakpoints based on content rather than specific devices
- Writing cleaner CSS with reusable patterns and design tokens
- Building confidence with Git and professional commit workflows
 
### Useful resources
 
- MDN Web Docs - Helpful for reviewing CSS properties, responsive images, Flexbox concepts, media queries, and accessibility features such as `:focus-visible`.
- Google Fonts - Used to load the Montserrat and Fraunces typefaces required by the project's style guide.
- Frontend Mentor - Provided the challenge, reference designs, assets, and style guide.
 
### AI collaboration
 
I used Microsoft 365 Copilot as a learning and development partner while completing this project.
 
Rather than having AI generate the completed project, I used it primarily to:
 
- Break the project into manageable development stages
- Explain HTML and CSS concepts while I implemented them
- Review responsive layout decisions
- Help troubleshoot problems
- Explain Git commands and workflow
- Review my work at different viewport sizes
- Help document what I learned
 
The most useful part of the process was working through the implementation incrementally while understanding why each technique was being used. I also learned that AI-generated suggestions still need to be reviewed carefully, especially when code formatting or implementation details do not behave as expected.
 
## Author
 
- Frontend Mentor - [\[Add Frontend Mentor profile\]](https://www.frontendmentor.io/profile/qcyrus8j562z1111)
- GitHub - [[Add GitHub profile\]](https://github.com/qcyrus8j562z1111)
