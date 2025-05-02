# ⚙️ Tailwind Setup — PostCSS

This folder demonstrates how to set up Tailwind CSS using **PostCSS**.

---

## 📦 What Is PostCSS?

PostCSS is a tool that processes your CSS using JavaScript plugins.  
In this setup, PostCSS runs Tailwind and adds browser vendor prefixes automatically using `autoprefixer`.

---

## 📁 Files Included

- `index.html` – Simple HTML using Tailwind utility classes
- `input.css` – Tailwind directives
- `output.css` – Compiled file from PostCSS
- `tailwind.config.js` – Tailwind settings
- `postcss.config.js` – Tells PostCSS to use Tailwind and Autoprefixer

---

## 🚀 How to Run It

1. Install the required tools:

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init
```

2. Then build your CSS:

```bash
npx postcss input.css -o output.css
```

3. Open `index.html` in your browser.

✅ Tailwind + PostCSS setup is commonly used in frameworks like Laravel Mix, Vue CLI, and more.

---

## 🧠 Why Use PostCSS?

- You can chain multiple PostCSS plugins (e.g., nesting, minification).
- Tailwind integrates natively as a PostCSS plugin.
- Easily used in production pipelines.

---

## ⚠️ Plugin Change (Tailwind v4+)

If you're using **Tailwind CSS v4.x or later**, the PostCSS plugin has moved to a separate package.

✅ Be sure to install this instead:

```bash
npm install -D @tailwindcss/postcss
```

Then use it in your `postcss.config.js` like this:

```js
module.exports = {
  plugins: {
    "@tailwindcss/postcss": {},
    autoprefixer: {},
  },
};
```

This change is necessary because the main `tailwindcss` package no longer exports a PostCSS plugin directly.
