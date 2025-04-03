# HTML (HyperText Markup Language)

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