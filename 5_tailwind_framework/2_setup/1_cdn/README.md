# 🌐 Tailwind Setup — CDN

## 🧪 What is This?

This folder demonstrates the **simplest way to use Tailwind CSS** — by loading it from a CDN.

## 🚀 How It Works

You include this line in your `<head>`:

```html
<script src="https://cdn.tailwindcss.com"></script>
```

✅ This loads Tailwind’s utility classes directly into the page.  
✅ No build process is needed.  
✅ Great for quick prototyping or HTML demos.

---

## 📂 Files

- `index.html` – A complete HTML page with Tailwind loaded via CDN
- No config files, no bundlers, no PostCSS needed.

---

## ❗ Limitations

- Not recommended for production (slightly larger file size, less customization).
- You can’t use advanced features like:
  - Just-in-Time compilation
  - Custom themes or plugins
  - Purging unused CSS

---

## ✅ When to Use This

- Learning Tailwind
- Creating simple HTML mockups
- Prototyping in CodePen or JSFiddle