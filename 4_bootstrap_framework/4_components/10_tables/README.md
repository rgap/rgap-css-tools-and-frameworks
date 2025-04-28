# 📘 Bootstrap Components — Tables

## 🕰️ Historical Context

Before Bootstrap, styling tables involved:

- Writing custom CSS for borders, padding, and row coloring.
- Handling responsiveness separately.

✅ Bootstrap standardized **Tables** with simple classes for clean, consistent designs.

---

## 📦 How Bootstrap Tables Work

Tables use a basic `<table>` structure enhanced with classes:

| Purpose          | Class Example      |
| :--------------- | :----------------- |
| Table container  | `table`            |
| Striped rows     | `table-striped`    |
| Hoverable rows   | `table-hover`      |
| Bordered table   | `table-bordered`   |
| Responsive table | `table-responsive` |

✅ Base class is **`table`**.
✅ Additional classes modify style and behavior.

---

## 📄 Basic Table Example

```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@motto</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```

✅ Clean table with default spacing and borders.

---

## 🔧 How Bootstrap Enhances Tables

- Consistent spacing and padding.
- Optional row striping, hover effects, borders.
- Responsive wrapping for small screens.

---

## 💡 Quick Concept

Table = **`table`** + _(optional)_ enhancements like `table-striped`, `table-hover`, `table-bordered`, `table-responsive`.

---

## 💸 Why Bootstrap Tables Are Useful

- Save time on complex table styling.
- Better readability and layout for tabular data.
- Responsive support with simple classes.
