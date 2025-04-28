# 📘 Bootstrap Grid System — Basic Structure

## 🕰️ Historical Context

Before Bootstrap, creating multi-column layouts involved:

- Using **tables** (bad practice for layout)
- Complex **float-based hacks**
- Custom CSS frameworks that were inconsistent

✅ Bootstrap introduced a **simple 12-column grid** using only CSS classes,  
making layout predictable, responsive, and flexible.

---

## 📦 How Bootstrap's Grid System Works

- **Container**: A fixed-width or fluid wrapper around the content.
- **Row**: A horizontal group for organizing columns.
- **Column**: Divides space into 12 equal parts (can span multiple parts).

✅ Think of every row as divided into **12 units** total.

---

## 📄 Basic Example

```html
<div class="container">
  <div class="row">
    <div class="col-6">50% width</div>
    <div class="col-6">50% width</div>
  </div>
</div>
```

✅ Two columns, each occupying **6 units** out of 12 ➔ equal split.

---

## 🧠 Key Rules

- `.col-6` means **6/12** = 50% width
- `.col-4` means **4/12** = 33.3% width
- `.col-12` means full width (100%)
- Columns **must always be inside rows** for proper alignment.

✅ If the total column span exceeds 12, Bootstrap wraps to the next line automatically.

---

## ⚡ Quick Concept

- Create a **container**
- Add a **row**
- Divide the row into **columns adding up to 12**

✅ Easy to scale for simple or complex layouts!

---
