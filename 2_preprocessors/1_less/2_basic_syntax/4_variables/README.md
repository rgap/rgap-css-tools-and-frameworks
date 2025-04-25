# 📘 LESS Variables

## 🧠 What This File Shows

This example introduces **variables in LESS**, one of the most important and widely used features.

## ✨ What are variables?

Variables in LESS start with an `@` symbol and allow you to store and reuse values like:

- Colors
- Fonts
- Spacing
- Sizes

They make your code more maintainable and consistent.

## ✅ Example

```less
@main-color: #4caf50;
@font-stack: "Segoe UI", sans-serif;
@padding: 16px;

body {
  color: @main-color;
  font-family: @font-stack;
  padding: @padding;
}
```
