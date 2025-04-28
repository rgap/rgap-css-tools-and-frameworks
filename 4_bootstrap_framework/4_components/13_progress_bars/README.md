# 📘 Bootstrap Components — Progress Bars

## 🕰️ Historical Context

Before Bootstrap, creating animated and styled progress bars meant:

- Writing custom CSS for widths, background colors, and animations.
- Handling accessibility manually.

✅ Bootstrap simplified **Progress Bars** with easy classes and built-in features.

---

## 📦 How Bootstrap Progress Bars Work

Progress bars are containers with inner bars:

| Purpose            | Class Example  |
| :----------------- | :------------- |
| Progress container | `progress`     |
| Inner progress bar | `progress-bar` |

✅ Set the width of the bar with inline `style="width: X%;"`.
✅ Accessibility attributes like `aria-valuenow`, `aria-valuemin`, `aria-valuemax` are recommended.

---

## 📄 Basic Progress Bar Example

```html
<div class="progress">
  <div class="progress-bar" role="progressbar" style="width: 50%;" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100">50%</div>
</div>
```

✅ Displays a half-filled progress bar.

---

## 📄 Progress Bar with Color

```html
<div class="progress">
  <div class="progress-bar bg-success" role="progressbar" style="width: 75%;" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">75%</div>
</div>
```

✅ Adds color (e.g., green for success).

---

## 🔧 How Bootstrap Enhances Progress Bars

- Easy to stack multiple progress bars inside one container.
- Custom colors (`bg-primary`, `bg-success`, `bg-danger`, etc.).
- Striped and animated variations available.

---

## 💡 Quick Concept

Progress Bar = **`progress`** + **`progress-bar`** + **inline width**.

---

## 💸 Why Bootstrap Progress Bars Are Useful

- Easy to show task completion visually.
- Built-in support for colors, stripes, animations.
- Fully responsive and accessible.
