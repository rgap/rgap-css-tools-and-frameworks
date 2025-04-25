# 📘 Nesting in LESS

## 🧠 What This File Demonstrates

LESS allows you to **nest CSS rules** inside selectors, following the structure of your HTML.

## ✅ Example

````less
article {
  h2 {
    color: blue;
  }
}

Compiles to:

```css
article h2 {
  color: blue;
}
````

## 📌 Why It's Useful

- Keeps related styles visually grouped
- Reflects HTML structure
- Reduces duplication in complex layouts
