# 📘 Bootstrap Components — Toasts

## 🕰️ Historical Context

Before Bootstrap, creating lightweight, non-blocking alerts ("toasts") meant:

- Manual CSS/JS for positioning, fade-in, fade-out.
- No consistent cross-browser behavior.

✅ Bootstrap introduced **Toasts** as ready-to-use notification components.

---

## 📦 How Bootstrap Toasts Work

Toasts are lightweight notification messages:

| Purpose         | Class Example  |
| :-------------- | :------------- |
| Toast container | `toast`        |
| Toast header    | `toast-header` |
| Toast body      | `toast-body`   |

✅ Toasts are hidden by default and can be shown with JavaScript.
✅ Built-in fade animations and accessibility attributes.

---

## 📄 Basic Toast Example

```html
<!-- Button to show Toast -->
<button type="button" class="btn btn-primary" id="showToastBtn">Show Toast</button>

<!-- Toast Structure -->
<div class="position-fixed bottom-0 end-0 p-3" style="z-index: 11">
  <div id="liveToast" class="toast" role="alert" aria-live="assertive" aria-atomic="true">
    <div class="toast-header">
      <strong class="me-auto">Bootstrap</strong>
      <small>Just now</small>
      <button type="button" class="btn-close" data-bs-dismiss="toast" aria-label="Close"></button>
    </div>
    <div class="toast-body">Hello, this is a Bootstrap Toast!</div>
  </div>
</div>
```

✅ Button triggers the toast programmatically.
✅ Toast can be closed manually or automatically if configured.

---

## 🔧 How Bootstrap Enhances Toasts

- Smooth animations (fade in, fade out).
- Auto-dismiss functionality.
- Customizable headers, body, and positioning.

---

## 💡 Quick Concept

Toast = **`toast`** + **`toast-header`** + **`toast-body`** + JavaScript control.

---

## 💸 Why Bootstrap Toasts Are Useful

- Non-intrusive way to deliver messages.
- Better user experience than modals for quick alerts.
- Mobile-friendly and lightweight.
