# 📘 Bootstrap Components — Buttons

## 🕰️ Historical Context

Before Bootstrap, creating consistent buttons across different browsers required:

- Writing custom CSS for each button type
- Dealing with inconsistent browser defaults (padding, borders, etc.)
- Managing hover, active, and focus states manually

✅ Bootstrap standardized button styling with a set of predefined classes.  
Developers could easily apply consistent design, color schemes, and sizes without writing extra CSS.

---

## 📦 How Bootstrap Buttons Work

Bootstrap provides a **base button class** `.btn`, and then **variant classes** like:

| Button Type      | Class               | Purpose                           |
| :--------------- | :------------------ | :-------------------------------- |
| Primary          | `btn btn-primary`   | Main action                       |
| Secondary        | `btn btn-secondary` | Alternative action                |
| Success          | `btn btn-success`   | Positive outcome                  |
| Danger           | `btn btn-danger`    | Negative outcome                  |
| Warning          | `btn btn-warning`   | Caution                           |
| Info             | `btn btn-info`      | Informational                     |
| Light            | `btn btn-light`     | Light background buttons          |
| Dark             | `btn btn-dark`      | Dark background buttons           |
| Link (text link) | `btn btn-link`      | Styled as link, not a real button |

✅ Each button type gives semantic meaning and visual distinction to actions.

---

## 📄 Example: Basic Buttons

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Danger</button>
```

✅ Notice:

- All buttons share `.btn`
- Variant (color) comes from the second class like `.btn-primary`

---

## 🎛️ Button Sizes

Bootstrap also allows **size adjustments**:

| Size  | Class        | Effect          |
| :---- | :----------- | :-------------- |
| Large | `btn btn-lg` | Bigger buttons  |
| Small | `btn btn-sm` | Smaller buttons |

✅ Easily adapt buttons to different UI needs.

---

## 📋 Additional Options

- **Block buttons**: Full-width buttons using `w-100`
- **Disabled state**: Add `disabled` attribute or `.disabled` class
- **Outline buttons**: Use `btn-outline-*` variants for minimal styling

Example outline button:

```html
<button class="btn btn-outline-primary">Primary Outline</button>
```

✅ Outline buttons have no background color until hover.

---

## ⚡ Quick Concept

Button = **`.btn`** + **variant class** (like `btn-primary`)
