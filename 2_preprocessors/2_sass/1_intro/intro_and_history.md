# 📘 Introduction to SASS / SCSS

## 🕰️ Historical Background

**SASS (Syntactically Awesome Stylesheets)** was introduced in **2006** by Hampton Catlin and further developed by Natalie Weizenbaum.

It was the **first widely adopted CSS preprocessor**, offering features that didn’t exist in native CSS:

- Variables
- Nesting
- Mixins
- Functions
- Partials and imports
- Logic: conditionals, loops

In 2010, the SCSS syntax was introduced — a CSS-compatible alternative to the original indentation-based syntax. Today, **SCSS is the most commonly used form of SASS**.

---

## 📌 Key Features

- `$variables`: Reusable values
- `@mixin` and `@include`: Reusable groups of rules
- Nesting: Write styles that mirror HTML structure
- Logic: `@if`, `@for`, `@each`, `@while`
- `@import` and `@use`: Code splitting and reuse

---

## 💡 Why Use SASS?

- DRY code (Don't Repeat Yourself)
- Easier to manage large stylesheets
- Framework support (Bootstrap, Foundation, etc.)
- Supported by modern bundlers like Webpack, Vite

---

## 🔍 SASS / SCSS vs Native CSS

| Feature   | Native CSS   | SASS (.sass)     | SCSS (.scss) |
| --------- | ------------ | ---------------- | ------------ |
| Variables | ✅ (limited) | ✅               | ✅           |
| Nesting   | 🧪 (limited) | ✅               | ✅           |
| Mixins    | ❌           | ✅               | ✅           |
| Logic     | ❌           | ✅               | ✅           |
| Modules   | ✅ (new)     | ✅ (with `@use`) | ✅           |

---

## 🔧 How to Compile

Install SASS via npm:

```bash
npm install -g sass
```

Compile your SCSS file:

```bash
sass styles.scss styles.css
```

---

## 🤔 Why Are There Two Syntaxes?

| Syntax   | Extension | Style             | Notes                                      |
| -------- | --------- | ----------------- | ------------------------------------------ |
| **SASS** | `.sass`   | Indentation-based | No `{}` or `;` — concise but less familiar |
| **SCSS** | `.scss`   | CSS-like syntax   | Fully compatible with CSS — widely used    |

Both syntaxes compile the same way and offer the same features.  
**SCSS is more common today** because it’s easier to adopt from plain CSS.

---

## 🆚 SCSS vs LESS (Quick Comparison)

| Feature           | LESS (2009)            | SCSS (2010)                        |
| ----------------- | ---------------------- | ---------------------------------- |
| Variables         | `@color`               | `$color`                           |
| Mixins            | `.mixin()`             | `@mixin` / `@include`              |
| Nesting           | ✅                     | ✅                                 |
| Functions         | Basic math, color ops  | Math + logic (`if`, `for`, `each`) |
| Extends           | `.class:extend()`      | `@extend .class`                   |
| Imports           | `@import`              | `@use` / `@import`                 |
| Native CSS syntax | ✅                     | ✅                                 |
| Adoption in tools | Popular (Bootstrap v2) | Standard (Bootstrap v4+)           |

## 💬 SCSS became dominant due to:

- Broader feature set (logic, modules)
- Community support
- Compatibility with modern tools and frameworks
