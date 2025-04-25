# 📘 Mixins in Stylus

## 🧠 What This Demonstrates

Stylus **mixins** allow you to define reusable blocks of CSS.

You define a function-like style block, then call it where needed.

---

## ✅ Example

```stylus
button-style()
  padding 10px
  background blue
  color white

.button
  button-style()
```

## 💡 Why Use Mixins?

- Follow DRY (Don't Repeat Yourself) principle
- Reuse common design patterns easily
- Accept arguments for dynamic styles
