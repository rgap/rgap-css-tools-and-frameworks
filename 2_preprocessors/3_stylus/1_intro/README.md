# 🎨 Simplest Stylus Example

This is the most basic example of using **Stylus** to define a color variable and apply it to a CSS rule.

---

## 📄 `styles.styl`

```stylus
$primary-color = blue

body
  background-color $primary-color
```

This Stylus file defines a variable `$primary-color` and uses it to set the background color of the `<body>` element.  
Notice there are **no semicolons** and **no braces** — indentation alone defines the structure.

---

## ⚙️ How to Compile

First, make sure you have Stylus installed:

```bash
npm install -g stylus
```

Then compile your `.styl` file to `.css`:

```bash
stylus styles.styl
```

It will automatically generate a `styles.css` file.

---

## 📄 Output: `styles.css`

```css
body {
  background-color: blue;
}
```

This is the final CSS output that your browser can understand.

---

✅ You are now using Stylus! 🎉
