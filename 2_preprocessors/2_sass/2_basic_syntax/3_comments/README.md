# 📘 Comments in SCSS

## ✍️ Two Types of Comments

SCSS supports both:

1. `// Single-line comments`

   - Used during development
   - ❌ These are **not included** in the final CSS

2. `/* Multi-line comments */`

   - ✅ These **do appear** in the compiled CSS
   - Useful for documentation or license banners

---

## ✅ Example Recap

```scss
// This is ignored by the compiler
/* This will appear in output */
```

## 💡 Best Practices

- Use // for quick dev notes and debugging
- Use /\* \*/ for output that needs to remain visible (e.g. attribution, docs)
