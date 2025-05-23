# 🛠️ Tailwind Setup — CLI

## ⚙️ What is This?

This project demonstrates how to set up and use **Tailwind CSS via the CLI** (Command Line Interface).  
It compiles custom utility-based styles using your own HTML and configuration, giving you **full control without needing a bundler** like Webpack or Vite.

This is the simplest way to get started with Tailwind in a real project.

---

## 📦 Step-by-Step Setup Guide

### 1. Install Tailwind CSS

Open your terminal in this project folder and run:

```bash
npm install -D tailwindcss@3.4.1
npx tailwindcss init
```

- `npm install -D tailwindcss@3.4.1` installs Tailwind (stable version) locally in your project (as a development dependency).
- `npx tailwindcss init` creates a basic `tailwind.config.js` file, which tells Tailwind where to look for class names.

---

### 2. Create Your Input CSS

File: `input.css`

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

These directives tell Tailwind to inject its:

- **Base layer** (`@tailwind base`) – includes Preflight (a CSS reset) and normalized styles for elements like `html`, `body`, `h1`, `ul`, etc.
- **Component layer** (`@tailwind components`) – includes any plugin-based or custom component styles if defined.
- **Utility layer** (`@tailwind utilities`) – injects Tailwind’s utility classes like `text-center`, `p-4`, `bg-blue-500`, etc.

✅ You can remove any of the three if you want to limit your CSS output.

---

### 3. Build Your CSS

Run this command to build Tailwind from your `input.css` into a real CSS file:

```bash
npx tailwindcss -i ./input.css -o ./output.css --watch
```

- `-i` specifies the input file (your raw directives).
- `-o` defines the output CSS file Tailwind will generate.
- `--watch` keeps the process running and rebuilds your CSS whenever you change your HTML or CSS files.

---

### 4. Open Your HTML

Now open `index.html` in your browser.  
It links to `output.css`, which was generated by Tailwind using only the classes found in `index.html`.

---

## 📄 File Overview

| File                 | Description                                                                    |
| -------------------- | ------------------------------------------------------------------------------ |
| `index.html`         | Basic HTML file using Tailwind classes like `bg-blue-500`, `text-center`, etc. |
| `input.css`          | Contains Tailwind's core directives (`@tailwind base`, etc.)                   |
| `output.css`         | The result of building Tailwind – contains actual compiled styles              |
| `tailwind.config.js` | Configuration file telling Tailwind where to scan for class usage              |
| `README.md`          | You’re reading it! Full guide to how this setup works                          |

---

## 🔍 Why Use the CLI Approach?

This CLI setup is ideal when you:

- Don’t want to use a bundler like Vite or Webpack
- Want full control over the build
- Are working on a static site or learning environment
- Prefer minimal dependencies

It’s lightweight, portable, and gives you the full power of Tailwind with very little setup.

---

## 🧪 Useful Tips

- You can customize Tailwind's default theme by editing `tailwind.config.js`.
- You can also create custom components using `@layer components` in your CSS.
- When ready for production, remove `--watch` and add CSS purging via `purge`/`content` settings in `tailwind.config.js`.

---

## 🚀 Next Steps

- Try editing `index.html` and adding new utility classes.
- Watch how the styles update instantly while `--watch` is running.
- Explore Tailwind’s docs to go deeper: https://tailwindcss.com/docs
