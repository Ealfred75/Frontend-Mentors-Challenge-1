# Frontend Mentor - QR Code Component Solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Overview

A simple yet elegant QR code component built with semantic HTML5 and CSS. The design features a centered card with a QR code image, heading, and descriptive text. This project demonstrates fundamental CSS concepts including layout, typography, and responsive design.

### Screenshot

![QR Code Component](project%20screenshot.jpeg)

## My Process

### Built With

- Semantic HTML5 markup
- CSS3 with Flexbox
- Mobile-first workflow
- Google Fonts (Outfit typeface)
- HSL color values for accessibility

### What I Learned

#### 1. **CSS Reset with Universal Selector**

Starting with a global CSS reset using the universal selector (`*`) was a game-changer. This resets default margins, padding, and box-sizing across all elements:

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

This prevents unexpected spacing issues and makes it easier to control padding and margins precisely on specific elements. It's a professional best practice that saves a lot of debugging time.

#### 2. **Understanding the Box Model Through Padding and Margin**

This project reinforced the difference between padding and margin:
- **Padding** adds space *inside* the element (between content and border)
- **Margin** adds space *outside* the element (between elements)

```css
.container {
  padding: 20px;  /* Space inside the card */
  margin: auto;   /* Space outside to center */
}
```

By controlling these separately, I could create the exact spacing the design required.

#### 3. **Flexbox for Centering**

I discovered that Flexbox is the ideal tool for centering content both vertically and horizontally:

```css
body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  min-height: 100vh;
}
```

This single approach eliminates the frustration of trying to center elements without it.

#### 4. **Using CSS Pseudo-selectors**

I used `:first-child` and `:last-child` selectors to target specific paragraphs without adding extra classes:

```css
.description p:first-child {
  font-size: 22px;
  font-weight: 700;
}

.description p:last-child {
  font-size: 15px;
  font-weight: 400;
}
```

This keeps the HTML cleaner while providing precise CSS control.

#### 5. **Responsive Design Considerations**

Using `max-width` instead of fixed `width` made the component responsive:

```css
.container {
  width: 100%;
  max-width: 375px;
}
```

This allows the card to scale on smaller screens while maintaining a fixed maximum width on larger ones.

### Continued Development

In future projects, I want to:
- Learn and practice **CSS Grid** for more complex layouts
- Explore **media queries** for true responsive design across all screen sizes
- Understand **CSS variables** (custom properties) for maintainable color and spacing systems
- Master **advanced Flexbox** techniques like `gap`, `wrap`, and alignment properties
- Practice building layouts **without default resets**, relying on semantic HTML more

### Useful Resources

- [MDN: CSS Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model) - Deep dive into padding, margin, and borders
- [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Visual explanations of Flexbox properties
- [Google Fonts: Outfit](https://fonts.google.com/specimen/Outfit) - The font used in this project
- [Coolors.co](https://coolors.co/) - Helpful for understanding HSL color values
- [FreeCodeCamp Responsive Design Course](https://www.freecodecamp.org/) - Where I'm learning responsive web development

### AI Collaboration

I used **GitHub Copilot** as a mentor during this project. Rather than giving me complete solutions, the AI guided me through hints and asked clarifying questions that helped me learn:

- **What worked well:** The AI provided guidance at the right pace, asking me questions before revealing solutions. This forced me to think through problems rather than copying code.
- **The process:** I would describe what I wanted to achieve, and the AI would ask what I'd already tried and guide me toward the solution with hints.
- **Learning outcome:** This approach reinforced my understanding of CSS concepts because I had to apply them myself rather than just copy-pasting code.

The mentoring style was especially helpful as a beginner—I learned *how* to think through CSS problems rather than just *what* the code should be.

## Author

- Frontend Mentor - [@Ealfred75](https://www.frontendmentor.io/profile/Ealfred75)
- GitHub - [github.com/Ealfred75](https://github.com/Ealfred75)

## Acknowledgments

Thanks to Frontend Mentor for the challenge design and specifications that made this realistic learning experience possible.


