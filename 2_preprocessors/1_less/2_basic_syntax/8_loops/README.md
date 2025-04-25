# 📘 Loops in LESS (Recursive Mixins)

## ✨ What This File Demonstrates

LESS doesn’t have traditional `for` loops, but you can achieve looping using **recursive mixins**.

## ✅ Example

```less
.loop(@i) when (@i > 0) {
  .margin-@{i} {
    margin: @i * 4px;
  }
  .loop(@i - 1);
}

.loop(5);
```

This generates:

```css
.margin-5 { margin: 20px; }
.margin-4 { margin: 16px; }
.margin-3 { margin: 12px; }
...
```

## 🧪 Use Case

Used to:

- Generate utility classes (e.g. spacing)
- Build consistent grids or typography steps
