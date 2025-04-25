# 📘 Conditionals in LESS (Guard Clauses)

## 🧠 What This Shows

LESS allows **conditional logic** inside mixins using `when` clauses.  
These are called **guarded mixins**.

## ✅ Example

```less
.text-color(@mode) when (@mode = dark) {
  color: white;
}
```

You can then apply it like this:

```less
.dark-mode {
  .text-color(dark);
}
```

## 🧪 Use Case

Use conditionals for:

- Themes (light vs dark)
- RTL vs LTR layouts
- Responsive styling variants
