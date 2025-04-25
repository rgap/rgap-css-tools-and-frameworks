# 📘 Imports and Partials in SCSS

## 🧠 What This File Shows

SCSS allows you to **split your styles into smaller files**, then import them.

---

## ✅ How It Works

- Files that start with an underscore (e.g., `_variables.scss`) are called **partials**
- They’re not compiled to standalone `.css` — only included where imported
- Use `@import 'filename'` without the underscore or extension

---

## 📂 Example

```scss
// styles.scss
@import "variables";
@import "mixins";

.container {
  @include card-style;
}
```

## 💡 Why Use This?

- Organize by purpose: variables, mixins, layout, components
- Reuse code across files
- Easy to maintain in large projects
