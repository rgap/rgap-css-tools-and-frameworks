# 📘 Bootstrap Components — Badges

## 🕰️ Historical Context

Before Bootstrap, adding labels like "New", "99+", or "Sale" required:

- Custom CSS for font sizes, backgrounds, borders.
- Positioning tricks for inline or inside buttons.

✅ Bootstrap introduced **Badges** to quickly add lightweight, small visual indicators anywhere in the UI.

---

## 📦 How Bootstrap Badges Work

Bootstrap badges are **inline elements** (`<span>`) that use simple classes:

| Purpose               | Class Example                       |
| :-------------------- | :---------------------------------- |
| Basic badge           | `badge bg-primary`                  |
| Badge inside a button | `badge bg-danger position-absolute` |

✅ Base class is **`badge`**.
✅ Variant class like **`bg-primary`**, **`bg-success`**, **`bg-danger`** changes background color.
✅ Add **`rounded-pill`** to make badges rounded.

---

## 📄 Basic Badge Example

```html
<h1>Example Heading <span class="badge bg-secondary">New</span></h1>
```

✅ This adds a **small grey badge** next to a heading.

---

## 🔧 Badge Inside Button Example

```html
<button type="button" class="btn btn-primary position-relative">
  Notifications
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    5
    <span class="visually-hidden">unread messages</span>
  </span>
</button>
```

✅ The badge becomes a **small red counter** positioned over the button.
✅ Helps users see how many new notifications or items there are.

---

## 💡 Quick Concept

Badge = **`badge`** + **background color class** (`bg-primary`, `bg-danger`, etc.) + _(optional)_ **rounded shape**.

---

## 💸 Why Bootstrap Badges Are Useful

- Draw attention to small pieces of information.
- Enhance buttons, links, headings without complex CSS.
- Easily customizable and positionable.
