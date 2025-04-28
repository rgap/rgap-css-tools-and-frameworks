# 📘 rtlcss

## 🕰️ Historical Background

When building websites for **Right-To-Left (RTL)** languages like Arabic, Hebrew, or Persian, developers had to **manually flip** many CSS properties:

- `margin-left` → `margin-right`
- `padding-left` → `padding-right`
- `text-align: left` → `text-align: right`

✅ In **2012**, **rtlcss** was introduced to **automate this flipping process**, saving developers hours of manual work and mistakes.

---

## 📌 What rtlcss Does

- Automatically flips **directional CSS properties**
- Transforms **left/right values** correctly
- Works on **finished CSS files**

✅ No need to manually create two versions of your stylesheet!

---

## 📄 Example: `styles.css` (input)

```css
.container {
  margin-left: 20px;
  padding-left: 10px;
  text-align: left;
}
```

---

## ⚙️ After Processing with rtlcss

```css
.container {
  margin-right: 20px;
  padding-right: 10px;
  text-align: right;
}
```

✅ rtlcss flipped everything automatically for RTL layouts!

---

## 💬 Why Use rtlcss?

- Save time when building RTL sites
- Avoid manual flipping errors
- Maintain a single source of truth for styles
- Handle large codebases consistently

---

## 🛠 How to Process (Basic Command)

First, install rtlcss globally:

```bash
npm install -g rtlcss
```

Then process your file:

```bash
rtlcss styles.css styles.rtl.css
```

✅ This reads your `styles.css`, flips it, and outputs `styles.rtl.css`.
