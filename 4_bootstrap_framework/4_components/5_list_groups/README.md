# 📘 Bootstrap Components — List Groups

## 🕰️ Historical Context

Before Bootstrap, creating lists with specific styles (like hover effects, active states, or disabled items) required:

- Custom CSS for each type of list item.
- Manual control over spacing, coloring, and interactions.

✅ Bootstrap introduced **List Groups** to create easily styled lists with consistent behaviors.

---

## 📦 How Bootstrap List Groups Work

List Groups are built using `<ul>` and `<li>` elements with Bootstrap classes:

| Purpose              | Class Example              |
| :------------------- | :------------------------- |
| List group container | `list-group`               |
| List item            | `list-group-item`          |
| Active item          | `list-group-item active`   |
| Disabled item        | `list-group-item disabled` |

✅ Base container is **`list-group`**.
✅ Each child item gets **`list-group-item`**.
✅ Special states like **`active`** or **`disabled`** are optional.

---

## 📄 Basic List Group Example

```html
<ul class="list-group">
  <li class="list-group-item">First item</li>
  <li class="list-group-item">Second item</li>
  <li class="list-group-item">Third item</li>
</ul>
```

✅ Quickly creates a vertical list with borders and spacing.

---

## 🔧 Active and Disabled Items Example

```html
<ul class="list-group">
  <li class="list-group-item active" aria-current="true">Active item</li>
  <li class="list-group-item">Regular item</li>
  <li class="list-group-item disabled" aria-disabled="true">Disabled item</li>
</ul>
```

✅ "Active" items are highlighted.
✅ "Disabled" items are muted and not interactive.

---

## 💡 Quick Concept

List Group = **`list-group`** + multiple **`list-group-item`** + _(optional)_ **active/disabled states**.

---

## 💸 Why Bootstrap List Groups Are Useful

- Standardized list designs.
- Easy to highlight active selections.
- Useful for menus, sidebars, and item listings.
- Great base for more complex components like tabs and interactive lists.
