# 📘 Introduction to LESS

## 🕰️ Historical Background

LESS was created in **2009** by **Alexis Sellier** (aka _cloudhead_), and is recognized as one of the **first CSS preprocessors**. It introduced programming concepts to CSS, which was groundbreaking at the time.

Initially, LESS ran in the **browser using JavaScript**, but later transitioned to **Node.js** for improved performance and tooling.

---

## 📌 Key Features

- **Variables**: Define reusable values like colors and margins with `@name`.
- **Mixins**: Bundle sets of CSS rules into reusable blocks using `.mixin()`.
- **Nested Rules**: Write rules inside rules to mimic HTML structure.
- **Functions & Operations**: Perform color math, calculations, logic.
- **Imports**: Split your styles into modular, maintainable files.

---

## 💡 Why Use LESS?

- Pioneered many CSS features we now use natively.
- Less repetitive code with **DRY** principles.
- **CSS-like syntax** made it easy to adopt.
- Was famously used in **Bootstrap v2**, increasing its popularity.
- Though SASS eventually surpassed it, LESS remains simple and powerful.

---

## 🔍 LESS vs Plain CSS (2009)

| Feature   | Native CSS | LESS               |
| --------- | ---------- | ------------------ |
| Variables | ❌         | ✅ `@mainColor`    |
| Nesting   | ❌         | ✅ `div { p { } }` |
| Mixins    | ❌         | ✅ `.button()`     |
| Functions | ❌         | ✅ `darken()`      |
| Imports   | Partial    | ✅ Modular imports |

---

## 🔧 How It Works

1. Write `.less` files using the enhanced syntax.
2. Compile to `.css` using tools like:
   - Command Line (`lessc styles.less styles.css`)
   - GUI apps (Prepros, Koala)
   - Build tools (Webpack, Gulp, etc.)

