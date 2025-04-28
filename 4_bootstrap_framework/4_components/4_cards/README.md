# 📘 Bootstrap Components — Cards

## 🕰️ Historical Context

Before Bootstrap, grouping images, text, and links together required:

- Writing lots of custom div structures.
- Customizing spacing, borders, and shadow manually.
- Handling mobile responsiveness separately.

✅ Bootstrap introduced **Cards** as flexible and extensible containers for content.

---

## 📦 How Bootstrap Cards Work

Bootstrap cards are **structured containers** with optional headers, footers, images, and buttons:

| Purpose             | Class Example  |
| :------------------ | :------------- |
| Main card container | `card`         |
| Image inside card   | `card-img-top` |
| Card body (content) | `card-body`    |
| Card title          | `card-title`   |
| Card text           | `card-text`    |

✅ Base container is **`card`**.
✅ Inner elements like **`card-body`**, **`card-title`**, and **`card-text`** organize the content neatly.

---

## 📄 Basic Card Example

```html
<div class="card" style="width: 18rem;">
  <img src="https://via.placeholder.com/286x180" class="card-img-top" alt="Placeholder Image" />
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

✅ A clean, ready-to-use card without needing custom CSS.

---

## 🔧 What You Can Add to Cards

- Images (`card-img-top`, `card-img-bottom`)
- Lists (`list-group` inside cards)
- Links and buttons
- Headers and footers
- Background colors and borders

✅ Cards are extremely flexible to fit different UI needs.

---

## 💡 Quick Concept

Card = **`card`** + **optional parts** (`card-body`, `card-title`, `card-text`, `card-img-top`, etc.).

---

## 💸 Why Bootstrap Cards Are Useful

- Organize information clearly.
- Reusable for product listings, blog posts, profiles, etc.
- Responsive by default with Bootstrap's grid system.
- Minimal custom CSS required.
