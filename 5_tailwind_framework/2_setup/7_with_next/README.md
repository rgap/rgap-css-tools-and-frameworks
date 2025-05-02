# 🧪 Tailwind CSS — With Next.js

This example shows how to set up **Tailwind CSS** in a **Next.js** project.

---

## 📜 Background

Since 2020, Tailwind CSS has supported integration with **Next.js** via **PostCSS**.

You can use utility classes directly in React components without configuring CSS Modules or writing separate `.css` files (except the global one).

---

## ⚙️ Setup Overview

Tailwind is installed as a PostCSS plugin and configured via:

- `tailwind.config.js`: specifies which files to scan
- `postcss.config.js`: connects Tailwind and Autoprefixer
- `styles/globals.css`: holds the Tailwind directives
- `pages/_app.js`: imports the CSS globally

---

## 🚀 How to Run

```bash
npm install
npm run dev
```

Then open: [http://localhost:3000](http://localhost:3000)
