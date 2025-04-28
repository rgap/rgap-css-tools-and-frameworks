# 📘 Autoprefixer

## 🕰️ Historical Background

Before Autoprefixer, developers had to **manually add vendor prefixes** to CSS properties to support different browsers, like:

```css
.container {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}
```

It was tedious, error-prone, and hard to maintain.

✅ **Autoprefixer**, introduced in **2013** by Andrey Sitnik, changed everything by **automatically adding vendor prefixes** based on real browser data.

---

## 📌 What Autoprefixer Does

- Parses your plain CSS
- Looks at browser support data (Can I Use database)
- Adds only the necessary vendor prefixes

✅ No more manual prefixes!

---

## 📄 Example: `styles.css` (input)

```css
.example {
  display: flex;
  user-select: none;
}
```

---

## ⚙️ After Processing with Autoprefixer

```css
.example {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;

  /*# sourceMappingURL=data:application/json;base64,... */
}
```

✅ Autoprefixer **added vendor-prefixed versions** of `user-select`,  
✅ while **keeping `display: flex` untouched** because modern browsers don't need prefixes for `flex` anymore.

---

## What is /_# sourceMappingURL=... _/?

When you run PostCSS (or Autoprefixer), it often adds a source map comment at the end of your output CSS.

✅ A source map links your compiled (processed) CSS back to your original CSS.
✅ It allows developer tools in the browser (like Chrome DevTools) to show you where each rule originally came from.
✅ Useful during development when debugging compiled CSS.

---

## 💬 Why This Example?

- **display: flex** → Already fully supported → ❌ No extra prefixes needed
- **user-select: none** → Needs prefixes for older Safari, Firefox → ✅ Prefixes added

✅ This proves that Autoprefixer is **smart**:  
it adds only what is **really necessary**, based on browser support data!

---

## 💬 Why Use Autoprefixer?

- Saves tons of time
- Reduces mistakes
- Keeps CSS clean and modern
- Only adds prefixes **when needed** (based on real browser versions)

---

## 🛠 How to Process (Basic Command)

First, make sure you have installed the needed tools:

```bash
npm install -g postcss postcss-cli autoprefixer
```

Then run Autoprefixer manually:

```bash
postcss styles.css --use autoprefixer -o styles.final.css
```

✅ This reads your `styles.css`, adds prefixes if needed, and outputs `styles.final.css`.
