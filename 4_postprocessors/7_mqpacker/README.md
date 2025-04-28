# 📘 mqpacker

## 🕰️ Historical Background

In large stylesheets, developers often ended up **scattering multiple identical media queries** across different places.

Example:

```css
@media (min-width: 768px) {
  .nav {
    display: block;
  }
}

... @media (min-width: 768px) {
  .footer {
    padding: 20px;
  }
}
```

✅ In **2014**, **mqpacker** was created to **combine identical media queries** into one block automatically.

This **makes the CSS smaller, faster, and easier to maintain**.

---

## 📌 What mqpacker Does

- Finds **identical media queries** throughout the CSS
- **Combines** all their contents into a **single media query block**
- Keeps CSS organized and optimized

✅ Helps browsers parse CSS faster and reduces file size!

---

## 📄 Example: `styles.css` (input)

```css
@media (min-width: 600px) {
  .header {
    font-size: 2rem;
  }
}

@media (min-width: 600px) {
  .footer {
    padding: 20px;
  }
}
```

---

## ⚙️ After Processing with mqpacker

```css
@media (min-width: 600px) {
  .header {
    font-size: 2rem;
  }
  .footer {
    padding: 20px;
  }
}
```

✅ mqpacker combined the two identical `@media (min-width: 600px)` blocks into one!

---

## 💬 Why Use mqpacker?

- Smaller CSS files
- Faster browser parsing
- Cleaner and more organized media queries
- Better production-ready CSS

---

## 🛠 How to Process (Basic Command)

First, install mqpacker globally:

```bash
npm install -g postcss postcss-cli css-mqpacker
```

Then run it manually:

```bash
postcss styles.css --use css-mqpacker -o styles.final.css
```

✅ This reads your messy `styles.css`, merges media queries, and outputs an optimized `styles.final.css`.

---

## ⚡ Quick Concept

Write **normal CSS** ➔ mqpacker ➔ **combined, optimized media queries**  
✅ No more duplicate media query blocks!
