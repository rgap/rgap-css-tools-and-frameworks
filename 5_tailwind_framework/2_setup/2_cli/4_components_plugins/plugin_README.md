# 🔌 Tailwind CLI — @tailwind components + Plugins

This folder demonstrates how to use the `@tailwind components` layer along with an official plugin: `@tailwindcss/forms`.

---

## 📦 What Plugin Is Used?

We’re using [`@tailwindcss/forms`](https://tailwindcss.com/docs/plugins#forms) to normalize and simplify default form styles.

It automatically applies better base styles to `<input>`, `<textarea>`, `<select>`, etc., so they look consistent and more polished across browsers.

---

## 🧩 How It Works

In `tailwind.config.js`:

```js
const forms = require('@tailwindcss/forms');

module.exports = {
  content: ["./index.html"],
  plugins: [forms],
}
```

- The plugin injects styles into the `@tailwind components` layer.
- It gives Tailwind a **better baseline** for form fields.
- You don’t need to manually style every form element — the plugin handles good defaults.

---

## 📄 Example Output

When you open the form in `index.html`, you’ll see:

- Inputs with clean borders
- Focused inputs with visible outlines
- No browser-inconsistent styles

These styles come from the plugin — **not from utility classes**.

---

## 📂 Files in This Folder

- `index.html` – A simple form
- `input.css` – Includes all Tailwind layers
- `tailwind.config.js` – Loads the forms plugin
- `output.css` – Generated file (after CLI run)

---

## 🚀 How to Run It

Install the plugin:

```bash
npm install -D @tailwindcss/forms
```

Then run:

```bash
npx tailwindcss -i ./input.css -o ./output.css --watch
```

✅ The form in your HTML will now have improved, normalized styles thanks to the plugin.
---

## ⚠️ Important Note on Plugin Styles

If you use only:

```css
@tailwind components;
```

...and your plugin injects styles into the **base layer** (like `@tailwindcss/forms` does), then **your output CSS may appear empty or incomplete**.

### ✅ Solution:
Include `@tailwind base;` along with `@tailwind components` in `input.css`:

```css
@tailwind base;
@tailwind components;
```

This ensures:
- Plugin styles injected into the base layer are actually included in your final CSS
- Form elements (like `<input>`, `<select>`, `<textarea>`) are styled correctly

Tailwind processes only the layers you explicitly declare — so if you leave out `@tailwind base`, you might miss key plugin styles.