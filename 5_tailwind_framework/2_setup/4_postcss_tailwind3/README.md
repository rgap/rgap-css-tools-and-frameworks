# ⚙️ Tailwind Setup — PostCSS (Tailwind v3.4.1)

This folder demonstrates how to use Tailwind CSS v3.4.1 with PostCSS.

---

## 📦 Packages Used

Install the required dependencies:

```bash
npm install -D tailwindcss@3.4.1 postcss autoprefixer
npx tailwindcss init
```

---

## 📁 Files

- `index.html` – A simple HTML file with Tailwind utility classes
- `input.css` – Contains Tailwind's layer directives
- `output.css` – Will be generated using PostCSS
- `tailwind.config.js` – Configures content scanning
- `postcss.config.js` – Loads Tailwind and Autoprefixer plugins

---

## 🛠 How It Works

PostCSS is a processor for CSS. It loads Tailwind as a plugin to:

- Compile `@tailwind` directives into real CSS
- Add vendor prefixes using Autoprefixer

---

### postcss.config.js

```js
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}
```

---

## 🚀 Build the CSS

After installing dependencies:

```bash
npx postcss input.css -o output.css
```

Then open `index.html` in your browser to see Tailwind in action.

✅ This setup is perfect for custom or framework-less builds using Tailwind v3.