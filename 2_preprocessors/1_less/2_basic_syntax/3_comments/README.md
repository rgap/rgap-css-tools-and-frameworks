# 📘 Comments in LESS

## ✍️ Two Types of Comments

LESS supports both:

1. `// Single-line comments`

   - These are **only used during development**
   - ❌ They are **not included** in the compiled `.css`

2. `/* Multi-line comments */`

   - These **are included** in the final CSS file
   - ✅ Good for CSS documentation or browser-visible comments

## 💡 Best Practices

- Use `//` for dev notes and debugging
- Use `/* */` if the comment needs to be seen in the browser or by other developers using the final CSS

## ✅ Example Recap

- The `body` rule uses both comment styles
- The `h1` rule includes a multi-line comment that would appear in production CSS
