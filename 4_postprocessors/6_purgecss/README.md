# 📘 PurgeCSS

## 🕰️ Historical Background

When websites started using frameworks like **Bootstrap** or **TailwindCSS**,  
developers realized that they were shipping **huge CSS files** —  
but often using only **10% of the classes**.

✅ **PurgeCSS**, introduced around **2017**, became the solution to **automatically remove unused CSS** based on your HTML and JavaScript files.

---

## 📌 What PurgeCSS Does

- Analyzes your HTML, JavaScript, or templates
- Detects which CSS classes are **actually used**
- Removes all unused styles from the final CSS

✅ It makes your stylesheets much smaller and faster to load!

---

## 📄 Example: `styles.css` (input)

```css
.used {
  color: green;
}

.unused {
  color: red;
}
```

---

## 📄 Example: `index.html`

```html
<div class="used">Hello!</div>
```

---

## ⚙️ After Processing with PurgeCSS

```css
.used {
  color: green;
}
```

✅ PurgeCSS removed `.unused` because it wasn’t found in `index.html`!

---

## 💬 Why Use PurgeCSS?

- Smaller CSS files
- Faster page loads
- Better Core Web Vitals
- Save bandwidth, improve SEO
- Professional production builds

---

## 🛠 How to Process (Basic Command)

First, install PurgeCSS globally:

```bash
npm install -g purgecss
```

Then run PurgeCSS manually:

```bash
purgecss --css styles.css --content index.html --output styles.final.css
```

✅ This reads your `styles.css`, checks which classes appear in `index.html`, and outputs only the used ones into `styles.final.css`.
