# 📘 postcss-preset-env

## 🕰️ Historical Background

Before **postcss-preset-env**, there was a tool called **cssnext** (2014–2017).  
**cssnext** allowed developers to **write future CSS today**, but it bundled everything together and eventually became hard to maintain.

✅ **postcss-preset-env** replaced cssnext —  
a more modular, flexible solution for using **future CSS features safely**.

---

## 📌 What postcss-preset-env Does

- Enables future CSS syntax safely (e.g., nesting, logical properties, new media queries)
- Adds polyfills only when needed
- Lets you control which CSS features are enabled

✅ You can use tomorrow’s CSS today — safely and modularly!

---

## 📄 Example: `styles.css` (input)

```css
.button {
  color: red;

  &:hover {
    color: blue;
  }
}
```

✅ This uses **nesting**, a future CSS syntax where you nest pseudo-classes like `:hover` directly inside rules.

---

## ⚙️ After Processing with postcss-preset-env

```css
.button {
  color: red;
}

.button:hover {
  color: blue;
}
```

✅ postcss-preset-env **unfolds** the nested structure into flat CSS that older browsers can understand.

✅ This proves how it automatically transforms modern CSS into compatible code!

---

## Where does it say &:hover will be allowed in CSS soon?

It comes from an official W3C draft called:

- [✅ CSS Nesting Module Level 1 (W3C Working Draft)](https://www.w3.org/TR/css-nesting-1/)
- It says that CSS will allow styles nested inside other rules, using & just like preprocessors!
- Tools like PostCSS, PostCSS Nesting, and others follow W3C drafts and browser progress closely.

---

## 💬 Why Use postcss-preset-env?

- Use modern CSS syntax safely
- Automatic polyfills for old browsers
- Customize which CSS features are enabled
- Future-proof your codebase while staying compatible

---

## 🛠 How to Process (Basic Command)

First, install the tools:

```bash
npm install -g postcss postcss-cli postcss-preset-env
```

Then process your file:

```bash
postcss styles.css --use postcss-preset-env -o styles.final.css
```

✅ This reads your modern `styles.css`, transforms it if needed, and outputs `styles.final.css`.
