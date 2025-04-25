# 📘 Variables in SCSS

## 🧠 What This File Shows

This example introduces **variables** in SCSS, one of its most useful features.

## ✨ What are Variables?

Variables start with a `$` and are used to store values like:

- Colors
- Fonts
- Sizes
- Spacing units

---

## ✅ Example

```scss
$main-color: #4caf50;
$font-stack: "Segoe UI", sans-serif;
$padding: 16px;

body {
  color: $main-color;
  font-family: $font-stack;
  padding: $padding;
}
```

## 📌 Why Use Them?

- Change a value in one place, and it updates everywhere
- Prevent mistakes from hardcoded values
- Supports theming and scaling your design system
