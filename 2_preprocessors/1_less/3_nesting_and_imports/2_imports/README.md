# 📘 Imports in LESS

## 🧠 What This File Demonstrates

LESS allows you to **split your code into separate files** using `@import`.

## ✅ Example

```less
@import "variables.less";
@import "mixins.less";
```

This makes all the variables and mixins defined in those files available here.

## 📌 Why It's Useful

- Helps organize large codebases
- Encourages modular styles
- Makes styles reusable across components

## 🔄 LESS vs Native CSS

- In LESS, @import brings in and compiles LESS syntax.
- In CSS, @import is for final .css files and is discouraged.
