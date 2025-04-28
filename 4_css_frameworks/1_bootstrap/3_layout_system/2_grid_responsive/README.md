# 📘 Bootstrap Grid System — Responsive Behavior

## 🕰️ Historical Context

Before mobile-first frameworks like Bootstrap, developers often:

- Created separate websites for desktop and mobile (m.site.com)
- Used JavaScript hacks for responsiveness
- Had poor adaptability across different screen sizes

✅ Bootstrap popularized the **mobile-first** philosophy,  
introducing **responsive breakpoints** directly into the grid system using simple classes.

---

## 📦 How Responsive Grid Works

Bootstrap's grid adapts layouts based on **screen width** using **breakpoints**:

| Breakpoint  | Class Prefix | Screen Size               |
| :---------- | :----------- | :------------------------ |
| Extra small | (none)       | `<576px` (default mobile) |
| Small       | `sm-`        | `≥576px`                  |
| Medium      | `md-`        | `≥768px`                  |
| Large       | `lg-`        | `≥992px`                  |
| Extra large | `xl-`        | `≥1200px`                 |
| XXL         | `xxl-`       | `≥1400px`                 |

✅ By using these prefixes, you can define **different column sizes** for different devices!

---

## 📄 Example: Responsive Columns

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6">Full width on mobile, 50% on desktop</div>
    <div class="col-12 col-md-6">Full width on mobile, 50% on desktop</div>
  </div>
</div>
```

✅ Explanation:

- On **small screens** (`<768px`): both columns take **full width** (`col-12`)
- On **medium and larger screens** (`≥768px`): columns split into **6 units** each (`col-md-6`)

---

## 🧠 Key Principles

- Always think **mobile-first** ➔ progressively adapt to larger screens.
- Combine classes (`col-`, `col-sm-`, `col-md-`) to control layout at different breakpoints.
- If you don’t define a size for a breakpoint, it inherits the previous one.

---

## ⚡ Quick Concept

Use **smaller prefixes** first (`col-12`) ➔ then **override** at larger breakpoints (`col-md-6`).  
✅ This makes layouts flexible and user-friendly across all devices.
