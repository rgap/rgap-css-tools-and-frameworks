# 📘 Bootstrap Components — Accordion

## 🕰️ Historical Context

Before Bootstrap, creating collapsible sections meant:

- Custom HTML, CSS, and JavaScript for open/close functionality.
- Managing multiple opened sections manually.

✅ Bootstrap provided **Accordion** as an organized way to collapse and expand content easily.

---

## 📦 How Bootstrap Accordion Works

Accordion is a container with collapsible items:

| Purpose                  | Class Example        |
| :----------------------- | :------------------- |
| Main container           | `accordion`          |
| Accordion item           | `accordion-item`     |
| Header button            | `accordion-button`   |
| Collapsible content area | `accordion-collapse` |

✅ Only one item is shown at a time if `data-bs-parent` is used.
✅ Uses Bootstrap's Collapse component internally.

---

## 📄 Basic Accordion Example

```html
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button
        class="accordion-button"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#collapseOne"
        aria-expanded="true"
        aria-controls="collapseOne"
      >
        Accordion Item #1
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
      <div class="accordion-body">This is the first item's accordion body.</div>
    </div>
  </div>
</div>
```

✅ Clicking the header toggles the content visibility.

---

## 🔧 How Bootstrap Enhances Accordions

- Handles multiple panels opening/closing automatically.
- Smooth transition animations.
- Accessible by keyboard and screen readers.

---

## 💡 Quick Concept

Accordion = **`accordion`** + **`accordion-item`** + **`accordion-button`** + **`accordion-collapse`**.

---

## 💸 Why Bootstrap Accordions Are Useful

- Organize large amounts of information.
- Great for FAQs, product info, menus.
- Saves screen space and improves user experience.
