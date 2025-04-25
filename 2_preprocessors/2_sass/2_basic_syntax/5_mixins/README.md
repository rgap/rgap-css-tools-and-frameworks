# 📘 Mixins in SCSS

## 🧠 What This File Shows

This example introduces **mixins**, a way to reuse groups of CSS declarations.

---

## ✨ What is a Mixin?

A mixin is like a function in CSS. You define it using `@mixin` and use it with `@include`.

### ✅ Example

```scss
@mixin button-style {
  padding: 10px;
  background: blue;
  color: white;
}

.button {
  @include button-style;
}
```

## 💡 Why Use Mixins?

- DRY principle: write once, reuse anywhere
- Great for utilities: cards, buttons, shadows, breakpoints
- Helps manage repeated patterns in your design system
