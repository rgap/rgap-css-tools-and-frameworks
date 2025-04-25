# 📘 Introduction to Stylus

## 🕰️ Historical Background

**Stylus** was introduced in **2010** by TJ Holowaychuk, a prolific Node.js developer known for projects like **Express.js**.

Stylus quickly attracted attention for its **highly flexible syntax**, allowing developers to write stylesheets in either an indentation-based style or a traditional CSS-like style — or mix both freely.

---

## 📌 Key Features

- `$variables`: Reusable values (similar to SASS)
- Mixins and **function-style mixins**
- Full **operator support** (`+`, `-`, `*`, `/`, `%`)
- Optional braces `{}`, semicolons `;`, and colons `:`
- Powerful built-in **functions** and **custom functions**
- Flexible **importing and modularization**

---

## 💡 Why Use Stylus?

- Minimalistic and flexible syntax
- Allows both clean, minimal code and standard CSS-like syntax
- Advanced function capabilities (beyond basic mixins)
- Great for developers who prefer **expressive** and **compact** stylesheets
- Easy integration with Node.js and frontend build systems

---

## 🔍 Stylus vs Native CSS

| Feature   | Native CSS   | Stylus                                    |
| --------- | ------------ | ----------------------------------------- |
| Variables | ✅ (limited) | ✅ More powerful                          |
| Nesting   | 🧪 (limited) | ✅ Full support                           |
| Mixins    | ❌           | ✅ Functions + Mixins                     |
| Logic     | ❌           | ✅ `if`, `for`, `each`, `while`           |
| Modules   | ✅ (new)     | ✅ with `@import` and flexible file usage |

---

## 🔧 How to Compile

Install Stylus globally:

```bash
npm install -g stylus
```

Compile your `.styl` file into `.css`:

```bash
stylus styles.styl
```

---

## 🤔 Why Is Stylus Syntax Flexible?

| Syntax Style        | Example                          | Notes               |
| ------------------- | -------------------------------- | ------------------- |
| Indented            | `body                            |
| color white`        | No braces `{}` or semicolons `;` |
| Braces & Semicolons | `body { color: white; }`         | Same as regular CSS |

You can mix both styles freely in a Stylus file.  
This flexibility is unique among preprocessors.

---

## 🆚 Stylus vs LESS vs SASS (Quick Comparison)

| Feature            | LESS (2009) | SASS/SCSS (2006/2010) | Stylus (2010)          |
| ------------------ | ----------- | --------------------- | ---------------------- |
| Syntax Flexibility | Low         | Medium                | Very High              |
| Variables          | `@color`    | `$color`              | `$color`               |
| Mixins             | `.mixin()`  | `@mixin`, `@include`  | Function-style mixins  |
| Nesting            | ✅          | ✅                    | ✅                     |
| Functions / Logic  | Basic math  | Full logic            | Full logic + operators |
| Import System      | `@import`   | `@import`, `@use`     | `@import` (flexible)   |
| Community Size     | Medium      | Very Large            | Small but focused      |

---

## 💬 Stylus remained a niche but loved tool because:

- It gives developers extreme syntax flexibility
- It is especially appreciated by **Node.js** and **JavaScript-centric** developers
- Ideal for projects that value **compactness** and **freedom of style**
