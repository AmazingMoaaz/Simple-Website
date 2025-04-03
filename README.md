- [HTML](#HTML) 
- [CSS](#CSS)

## HTML

HTML is the standard markup language for creating web pages. This documentation uses real examples from our tea shop website to demonstrate HTML elements and their usage.

## Document Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>My Tea Shop</title>
    <meta name="description" content="Welcome to our tea shop" />
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

## Headings
HTML provides six levels of headings, demonstrated in our tea shop sections:

```html
<h1>Welcome to Our Tea Shop</h1>
<h2>Our Tea Selection</h2>
<h3>Our Team</h3>
<h4>Departments</h4>
<h5>Product Details</h5>
<h6>Contact Info</h6>
```

## Semantic Elements
Semantic elements provide meaning to the structure:

```html
<header>
  <h1>Header Section</h1>
  <p>Welcome to our tea shop</p>
</header>

<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>

<article>
  <h2>Article Title</h2>
  <p>This is an article section about tea.</p>
</article>

<footer>
  <p>Footer Section</p>
</footer>
```

## Multimedia Elements

### Audio
```html
<audio controls>
  <source src="tea-audio.mp3" type="audio/mpeg" />
</audio>
```

### Video
```html
<video controls width="300">
  <source src="tea-video.mp4" type="video/mp4" />
</video>
```

### Images
```html
<img src="./tea-cup.png" alt="Tea Cup" />
```

## Forms
Our tea shop order form demonstrates various input types:

```html
<form>
  <!-- Text input -->
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required />

  <!-- Email input -->
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required />

  <!-- Password input -->
  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required />

  <!-- Number input -->
  <label for="age">Age:</label>
  <input type="number" id="age" name="age" />

  <!-- Date input -->
  <label for="birthdate">Birthdate:</label>
  <input type="date" id="birthdate" name="birthdate" />

  <!-- Color picker -->
  <label for="color">Favorite Color:</label>
  <input type="color" id="color" name="color" />

  <!-- File upload -->
  <label for="file">Upload File:</label>
  <input type="file" id="file" name="file" />

  <!-- Text area -->
  <label for="bio">Bio:</label>
  <textarea id="bio" name="bio"></textarea>

  <!-- Submit button -->
  <input type="submit" value="Submit" />
</form>
```

## Text Formatting
Examples from our tea descriptions:

```html
<p><strong>Bold Text</strong>: Tea is a popular beverage.</p>
<p><em>Italic Text</em>: Tea can be enjoyed hot or cold.</p>
<p><mark>Highlighted Text</mark>: Green tea is rich in antioxidants.</p>
<p><del>Deleted Text</del>: Black tea is not as healthy as green tea.</p>
<p><ins>Inserted Text</ins>: Herbal teas are caffeine-free.</p>
<p>H<sub>2</sub>O is essential for brewing tea.</p>
<p>100°C<sup>2</sup></p>
```

## Lists

### Unordered List (Tea Types)
```html
<ul>
  <li>Green Tea</li>
  <li>Black Tea</li>
  <li>
    Herbal Tea
    <ul>
      <li>Chamomile</li>
      <li>Peppermint</li>
      <li>Rooibos</li>
    </ul>
  </li>
</ul>
```

### Ordered List (Tea Information)
```html
<ol>
  <li>Tea ID</li>
  <li>Tea Name</li>
  <li>Origin</li>
</ol>
```

### Description List (Tea Descriptions)
```html
<dl>
  <dt>Green Tea</dt>
  <dd>Rich in antioxidants</dd>
  <dt>Black Tea</dt>
  <dd>Strong and bold flavor</dd>
</dl>
```

## Tables
Our tea pricing table:

```html
<table border="1">
  <caption>Tea Prices</caption>
  <thead>
    <tr>
      <th>Tea Name</th>
      <th>Price</th>
      <th>Quantity</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Green Tea</td>
      <td>$10</td>
      <td>50g</td>
      <td>Rich in antioxidants</td>
    </tr>
    <!-- More rows... -->
  </tbody>
  <tfoot>
    <tr>
      <td colspan="3">Total</td>
      <td>$30</td>
    </tr>
  </tfoot>
</table>
```

## Line Breaks and Horizontal Rules
```html
<p>This is the first line. <br />This is the second line.</p>
<hr />
```

## Accessibility Features
Our website implements these accessibility best practices:

1. Semantic HTML elements (`<header>`, `<nav>`, `<article>`, `<footer>`)
2. Proper heading hierarchy (`<h1>` to `<h6>`)
3. Alt text for images: `<img src="tea-shop.jpg" alt="Tea shop">`
4. Form labels with `for` attributes
5. ARIA roles and landmarks where needed

## Best Practices

1. **Document Structure**
   - Always include `<!DOCTYPE html>`
   - Use proper `<head>` and `<body>` sections
   - Include meta charset declaration

2. **Semantic Markup**
   - Use semantic elements instead of generic `<div>`
   - Maintain proper heading hierarchy
   - Use appropriate elements for content type

3. **Forms**
   - Always label form controls
   - Use appropriate input types
   - Include validation attributes when needed

4. **Accessibility**
   - Provide alt text for images
   - Use semantic elements
   - Maintain proper heading structure
   - Label form elements correctly

5. **Tables**
   - Use `<caption>` for table titles
   - Include proper table structure (`<thead>`, `<tbody>`, `<tfoot>`)
   - Use `<th>` for header cells

Remember:
- Always close your tags
- Use proper indentation
- Validate your HTML code
- Follow accessibility guidelines
- Keep your code clean and organized


---

## CSS

CSS is used to style HTML documents, controlling the visual presentation of web pages. Below is documentation of CSS concepts using examples from our tea shop website.

## CSS Integration Methods

### Inline CSS
```html
<p style="color: blue; font-size: 16px;">This text is blue and 16px in size.</p>
```

### Internal CSS (in the head section)
```html
<head>
  <style>
    p {
      color: #5c6b7a;
      margin-bottom: 2rem;
      font-size: 1.1rem;
    }
  </style>
</head>
```

### External CSS (separate file)
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

## CSS Selectors

### Basic Selectors
```css
/* Element selector */
nav {
  background-color: rgba(255, 255, 255, 0.95);
  padding: 2rem;
}

/* Class selector */
.container {
  max-width: 1200px;
  margin: 0 auto;
}

/* ID selector */
#about {
  background-color: white;
}

/* Universal selector */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

### Combinators
```css
/* Descendant selector (all paragraphs inside sections) */
section p {
  color: #5c6b7a;
}

/* Child selector (direct children only) */
nav > ul {
  list-style: none;
  display: flex;
}

/* Adjacent sibling selector */
h2 + p {
  font-weight: bold;
}

/* General sibling selector */
h2 ~ p {
  margin-top: 1rem;
}
```

### Attribute Selectors
```css
/* Elements with specific attribute */
input[type="text"] {
  border: 2px solid #dcd6c9;
}

/* Elements with attribute beginning with specific value */
a[href^="#"] {
  color: #8b5e3c;
}

/* Elements with attribute ending with specific value */
img[src$=".jpg"] {
  border-radius: 8px;
}

/* Elements with attribute containing specific value */
input[name*="tea"] {
  background-color: #fdf6e3;
}
```

### Pseudo-classes
```css
/* Style when hovering over element */
nav a:hover {
  color: #c17817;
}

/* Style for first child of its parent */
.tea-types article:first-child {
  border-left: 4px solid #e6a23c;
}

/* Style for nth child (even/odd or formula) */
tbody tr:nth-child(even) {
  background-color: rgba(139, 94, 60, 0.05);
}

/* Form element focus state */
input:focus {
  outline: none;
  border-color: #c17817;
}
```

### Pseudo-elements
```css
/* First line of paragraph */
p::first-line {
  font-weight: bold;
}

/* First letter of paragraph */
p::first-letter {
  font-size: 150%;
  color: #8b5e3c;
}

/* Content before an element */
h1::before {
  content: "☕ ";
}

/* Content after an element */
h1::after {
  content: "";
  display: block;
  width: 80px;
  height: 4px;
  background-color: #e6a23c;
  margin: 1rem auto 0;
}
```

## CSS Box Model

The box model consists of: content, padding, border, and margin.

```css
.box-model-example {
  /* Content dimensions */
  width: 300px;
  height: 200px;
  
  /* Padding (inner space) */
  padding: 20px;
  /* Or individual sides */
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-left: 20px;
  
  /* Border */
  border: 2px solid #dcd6c9;
  border-radius: 8px;
  
  /* Margin (outer space) */
  margin: 20px;
  /* Or individual sides */
  margin-top: 10px;
  margin-right: 20px;
  margin-bottom: 10px;
  margin-left: 20px;
}
```

## CSS Layout

### Display Properties
```css
/* Block elements (take full width) */
section {
  display: block;
}

/* Inline elements (take only necessary width) */
a {
  display: inline;
}

/* Inline-block (inline but with block properties) */
.nav-icon {
  display: inline-block;
  width: 20px;
  height: 20px;
}

/* Hidden elements */
.hidden-element {
  display: none;
}
```

### Flexbox
```css
/* Container */
nav ul {
  display: flex;
  justify-content: center; /* horizontal alignment */
  align-items: center; /* vertical alignment */
  gap: 4rem; /* space between items */
  flex-wrap: wrap; /* allows items to wrap */
}

/* Flex items */
nav li {
  flex: 1; /* grow and shrink proportionally */
}
```

### Grid
```css
/* Container */
.tea-types {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 4rem;
}

/* Grid placement */
.featured-item {
  grid-column: 1 / 3; /* spans from line 1 to line 3 */
  grid-row: 1 / 2; /* spans from line 1 to line 2 */
}
```

### Positioning
```css
/* Relative positioning */
.parent {
  position: relative;
}

/* Absolute positioning (relative to positioned parent) */
.child {
  position: absolute;
  top: 10px;
  right: 10px;
}

/* Fixed positioning (relative to viewport) */
.header {
  position: fixed;
  top: 0;
  width: 100%;
}

/* Sticky positioning (acts like relative until scrolled) */
nav {
  position: sticky;
  top: 0;
  z-index: 1000;
}
```

## CSS Variables (Custom Properties)

```css
/* Defining variables in root scope */
:root {
  --primary-color: #8b5e3c;
  --secondary-color: #c17817;
  --spacing-md: 2rem;
  --border-radius-md: 8px;
}

/* Using variables */
.button {
  background-color: var(--primary-color);
  padding: var(--spacing-md);
  border-radius: var(--border-radius-md);
}

/* Local variable scope */
.card {
  --card-padding: 16px;
  padding: var(--card-padding);
}
```

## Responsive Design

### Media Queries
```css
/* Base styles for all screen sizes */
.container {
  padding: 2rem;
}

/* Styles for screens smaller than 768px */
@media (max-width: 768px) {
  .container {
    padding: 1rem;
  }
  
  h1 {
    font-size: 2.5rem;
  }
  
  nav ul {
    flex-direction: column;
  }
}

/* Styles for print */
@media print {
  nav {
    display: none;
  }
  
  body {
    font-size: 12pt;
    color: black;
  }
}
```

### Fluid Units
```css
/* Percentage (relative to parent) */
.container {
  width: 80%;
}

/* Viewport units */
header {
  height: 100vh; /* 100% of viewport height */
  width: 100vw; /* 100% of viewport width */
}

/* Relative units */
p {
  font-size: 1.1rem; /* relative to root font size */
  line-height: 1.7; /* relative to element's font size */
}
```

## Transitions and Animations

### Transitions
```css
/* Basic transition */
.button {
  background-color: #c17817;
  color: white;
  transition: all 0.3s ease;
}

.button:hover {
  background-color: #8b5e3c;
  transform: translateY(-2px);
}

/* Individual property transitions */
nav a {
  transition-property: color, transform;
  transition-duration: 0.3s, 0.2s;
  transition-timing-function: ease, ease-out;
  transition-delay: 0s, 0.1s;
}
```

### Animations
```css
/* Defining keyframes */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Using animations */
.animated-element {
  animation-name: fadeIn;
  animation-duration: 1s;
  animation-timing-function: ease-out;
  animation-delay: 0.2s;
  animation-iteration-count: 1;
  animation-direction: normal;
  animation-fill-mode: forwards;
  
  /* Shorthand */
  animation: fadeIn 1s ease-out 0.2s 1 normal forwards;
}
```

## CSS Best Practices

1. **Organization**
   - Group related styles together
   - Use consistent naming conventions
   - Consider methodologies like BEM (Block Element Modifier)

2. **Efficiency**
   - Avoid overly specific selectors
   - Minimize use of `!important`
   - Understand the cascade and inheritance

3. **Maintainability**
   - Use CSS variables for reusable values
   - Break styles into logical components
   - Comment complex sections

4. **Performance**
   - Minimize use of expensive properties (box-shadow, border-radius)
   - Be careful with universal selectors
   - Optimize animations and transitions

5. **Responsive Design**
   - Design mobile-first
   - Use relative units
   - Test across multiple screen sizes

Remember:
- Keep CSS DRY (Don't Repeat Yourself)
- Consider browser compatibility
- Validate CSS
- Use CSS preprocessors for larger projects
- Always test design on multiple devices
