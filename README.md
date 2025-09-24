# Sass (SCSS) Project

This project demonstrates the use of **Sass (Syntactically Awesome Stylesheets)** to write better, modular, and more powerful CSS.  
Sass helps developers use **variables, nesting, mixins, partials, imports, and functions** to create maintainable stylesheets.

---

## 🚀 Getting Started

### 1️⃣ Install Sass
Make sure you have Node.js installed, then install Sass globally:
```bash
npm install -g sass
Check installation:

bash
Copy code
sass --version
2️⃣ Compile Sass
Compile SCSS into CSS manually:

bash
Copy code
sass style.scss style.css
Or watch files for automatic compilation:

bash
Copy code
sass --watch style.scss:style.css
You can also watch entire folders:

bash
Copy code
sass --watch scss:css
✨ Sass Features Used
Variables → Store reusable values (colors, fonts, sizes).

Nesting → Write CSS in a structured way inside parent selectors.

Mixins → Define reusable blocks of CSS.

Partials → Split code into smaller .scss files and import them.

Imports → Bring multiple SCSS files together.

Functions → Perform calculations and return values.

Extend/Inheritance → Share styles between selectors.

📂 Example Workflow
Write styles in style.scss (or multiple partials like _header.scss, _footer.scss).

Compile to style.css using sass.

Link the compiled style.css in your index.html.

Example in HTML:

html
Copy code
<link rel="stylesheet" href="style.css">
📘 Example SCSS
scss
Copy code
// Variables
$primary-color: #ff6f61;
$font-stack: 'Poppins', sans-serif;

// Mixin
@mixin flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

// Usage
body {
  font-family: $font-stack;
  background: $primary-color;
}

button {
  @include flex-center;
  padding: 10px 20px;
  border-radius: 5px;
  color: white;
  background: darken($primary-color, 10%);
}
📜 Best Practices
Use variables for colors, fonts, and spacing.

Break styles into partials for better organization.

Use mixins instead of repeating code.

Watch files during development (sass --watch).

Always compile SCSS before deploying to production.

