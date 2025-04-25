# 📘 Conditionals in Stylus

## 🧠 What This Demonstrates

Stylus allows you to use **`if`**, **`else if`**, and **`else`** logic directly inside your styles.

This makes your stylesheets dynamic and adaptable.

---

## ✅ Example

```stylus
theme($mode)
  if $mode == light
    background white
  else
    background black

.page
  theme(light)
```

## 💡 Why Use Conditionals?

- Create themes (light/dark mode)
- Adjust styles dynamically based on variables
- Avoid duplication and hardcoded alternatives
