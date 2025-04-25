# 🎨 Simplest SCSS & SASS Example

This is the most basic example of using **SCSS** and **SASS** to define a color variable and apply it to a CSS rule.

---

## 📄 `style.scss` (SCSS Syntax)

```scss
$primary-color: blue;

body {
  background-color: $primary-color;
}
```

This SCSS file defines a variable `$primary-color` and uses it to set the background color of the `<body>` element.  
It uses curly braces `{}` and semicolons `;`, similar to regular CSS.

---

## 📄 `style.sass` (SASS Syntax)

```sass
$primary-color: blue

body
  background-color: $primary-color
```

This SASS file does the exact same thing, but uses **indentation-based syntax** instead of curly braces and semicolons.

---

## ⚙️ How to Compile

First, make sure you have Dart Sass installed. You can install it globally with:

```bash
npm install -g sass
```

Then compile the SCSS or SASS file to CSS using:

```bash
# For SCSS
sass style.scss style.css

# For SASS
sass style.sass style.css
```

---

## 📄 Output: `style.css`

```css
body {
  background-color: blue;
}
```

This is the final CSS output that your browser can understand.

---

✅ You're now using SCSS and SASS! 🎉
