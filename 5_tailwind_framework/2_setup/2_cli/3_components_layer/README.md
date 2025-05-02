# 🧱 Tailwind CLI — @tailwind components

This folder demonstrates how to use only the `@tailwind components` directive with the Tailwind CLI.

---

## 🎯 What Is `@tailwind components`?

The `@tailwind components` directive is used to inject any **custom or plugin-based CSS components** into your compiled file.

- It’s a place to define your own class-based components (e.g., `.btn`, `.card`, etc.).
- You use `@layer components {}` to safely define your styles inside this layer.
- Unlike utility classes, component classes group multiple styles into one class name.

---

## ❗ Why It Matters

- Allows you to create **reusable abstractions** for common UI patterns.
- Helps keep your HTML cleaner by replacing long utility chains with a single semantic class.
- Works well with Tailwind plugins that inject styled components (like `@tailwindcss/forms`, etc.).

---

## 🛠️ How It Works in This Example

In `input.css`:

```css
@tailwind components;

@layer components {
  .btn-primary {
    @apply bg-blue-500 text-white font-semibold py-2 px-4 rounded hover:bg-blue-600;
  }
}
```

- `@tailwind components` injects the component layer.
- `@layer components` is where we define a **custom component class**.
- `.btn-primary` is now usable in your HTML just like a regular utility class, but it groups several Tailwind utilities together.

---

## 📄 Example Output

In the browser, you’ll see:

- A custom button that uses `.btn-primary`
- This class is made up of Tailwind utility styles grouped together

---

## 📂 Files in This Folder

- `input.css` – contains only `@tailwind components` + a custom class inside `@layer`
- `index.html` – uses `.btn-primary` to show a working example
- `output.css` – generated using Tailwind CLI
- `tailwind.config.js` – basic config that scans `index.html`

---

## 🚀 How to Run It

```bash
npx tailwindcss -i ./input.css -o ./output.css --watch
```

Then open `index.html` in your browser.

## ✅ You’ll see your custom `btn-primary` component in action.

## ⚠️ What Happens If You Use `@tailwind components` Alone?

If your `input.css` file contains only:

```css
@tailwind components;
```

...and you don't define any custom components using `@layer components {}` or install any Tailwind plugin, then **no component styles will be added to your output CSS**.

This is expected behavior because:

- Tailwind's component layer is **empty by default**.
- It is **meant for you or plugins to add styles into**.

---

### ✅ You’ll only see styles in your final CSS if:

1. You manually define component classes like:

```css
@layer components {
  .card {
    @apply p-4 bg-white shadow rounded;
  }
}
```

2. Or you enable a plugin that adds components:

```js
// tailwind.config.js
plugins: [require("@tailwindcss/forms")];
```

---

In short: **`@tailwind components` alone does nothing visually.** It’s a placeholder for you or plugins to fill.
