# 📘 Conditionals in SCSS

## 🧠 What This File Shows

SCSS supports **control flow** using `@if`, `@else if`, and `@else`.

You can add logic into your stylesheets to dynamically adjust output.

---

## ✅ Example

```scss
@mixin theme($mode) {
  @if $mode == light {
    background: white;
  } @else {
    background: black;
  }
}
```

# 🧪 Use Cases

- Theming (light vs dark)
- Layout direction (LTR vs RTL)
- Browser-specific or component-based logic
