# 📘 Tailwind CSS Preflight

## 🕰️ Historical Context

**Preflight** is a minimal CSS reset included by default in **Tailwind CSS**.  
It was introduced around **2017** by **Adam Wathan** to provide a "smart reset" based on **modern-normalize** but customized for utility-first CSS.

- 📖 Source: https://tailwindcss.com/docs/preflight

## 🎯 Purpose

Preflight aims to:

- Normalize styles across browsers
- Reset inconsistencies without removing everything useful
- Set sensible defaults like `box-sizing: border-box`
- Ensure all elements inherit base typography

## 🆚 Comparison to Normalize.css

| Feature                | Normalize.css | Tailwind Preflight |
| ---------------------- | ------------- | ------------------ |
| General purpose        | ✅            | Tailwind-specific  |
| Typography inheritance | ❌            | ✅                 |
| Utility-first focused  | ❌            | ✅                 |

## ✅ Use Cases

- Tailwind CSS projects
- Utility-first design systems
- Minimal custom CSS with maximum consistency

## 📁 Included Files

- `preflight.css`: Extracted simplified preflight stylesheet
- `index.html`: Demo showing preflight normalization
