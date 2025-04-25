# 📘 Nesting in LESS

## 🧠 What This Demonstrates

LESS allows **nesting CSS rules inside one another**, mimicking the hierarchy of HTML elements.

## ✅ Why It's Useful

- Reduces duplication (you don’t have to repeat the full selector path)
- Makes CSS more readable and maintainable

## ⚠️ Use Responsibly

Deep nesting (3+ levels) can become hard to debug or override. Stick to 1–2 levels for readability.

## 📁 Example

In the `2_nesting.less` file, we define styles for a navigation menu using **nested selectors**.

This structure:

```less
nav {
  ul {
    li {
      a {
        &:hover {
          ...;
        }
      }
    }
  }
}
```

is automatically compiled into regular CSS like this:

```css
nav ul li a:hover {
  ...;
}
```

## 💡 About &:hover

The & symbol refers to the current selector (a in this case).
So &:hover becomes a:hover when compiled.
