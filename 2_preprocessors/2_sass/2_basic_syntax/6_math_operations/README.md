# 📘 Math Operations in SCSS

## 🧠 What This File Demonstrates

SCSS allows you to do **math with units**, directly in your styles.

---

## ✨ Supported Operators

You can use:

- `+` addition
- `-` subtraction
- `*` multiplication
- `/` division
- `%` modulo

---

## ✅ Example

```scss
$base: 8px;

.padding-double {
  padding: $base * 2; // 16px
}

.margin-half {
  margin: $base / 2; // 4px
}
```

## 💡 Why Use This?

- Useful for spacing systems, layouts, font sizing, and grids
- Keeps values consistent and flexible
- Makes tokens scalable
