# 🎨 Simplest LESS Example

This is the most basic example of using LESS to define a color variable and apply it to a CSS rule.

---

## 📄 `styles.less`

```less
@primary-color: blue;

body {
  background-color: @primary-color;
}
```

This LESS file defines a variable `@primary-color` and uses it to set the background color of the `<body>` element.

---

## ⚙️ How to Compile

Make sure you have Node.js installed, then install LESS globally if you haven't:

```bash
npm install -g less
```

Then compile the LESS file to CSS using:

```bash
lessc styles.less styles.css
```

---

## 📄 Output: `styles.css`

```css
body {
  background-color: blue;
}
```

This output is regular CSS and can be used in your HTML files as usual.

---

✅ You're now using LESS! 🎉
