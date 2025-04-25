# 📘 Imports and Partials in Stylus

## 🧠 What This Demonstrates

Stylus allows you to **split styles into partials** and then import them into main files.

---

## ✅ Example

```stylus
@import 'variables'
@import 'mixins'

.page
  card-style()
```

## 📦 How Partials Work

- Files prefixed with \_ (e.g., \_variables.styl) are considered partials.
- You do not need to specify the underscore or file extension when importing.
- Partials are not compiled individually — only when imported.

## 💡 Why Use Imports?

- Organize styles by purpose
- Reuse code across different sections
- Easier team collaboration on large projects
