# 📘 modern-normalize.css

## 🕰️ Historical Context

**modern-normalize** was created by **Sindre Sorhus** in 2020 as a modern alternative to Normalize.css. As browser support matured, this tool was built to:

- Support only modern browsers (no Internet Explorer)
- Be smaller and faster than normalize.css
- Provide a clean base with modern best practices

## 🎯 Purpose

This reset:

- Assumes **modern CSS defaults** (e.g., `box-sizing: border-box`)
- Resets **margins** for common block elements
- Normalizes **form elements and images**
- Adds accessibility support (e.g., `prefers-reduced-motion`)
- Does not include outdated fixes or legacy browser rules

## 🆚 Comparison to Normalize.css

| Feature            | Normalize.css     | modern-normalize    |
| ------------------ | ----------------- | ------------------- |
| Size               | Larger            | Smaller             |
| Browser coverage   | Wide (incl. IE)   | Modern only (no IE) |
| Opinionated styles | Fewer             | Slightly more       |
| Maintainer         | Nicolas Gallagher | Sindre Sorhus       |

## ✅ Use Cases

- Projects that **only target modern browsers**
- Teams that want a **minimalist starting point**
- Static sites, JAMstack, Vite/React apps
- Replacing heavier resets in Tailwind, Parcel, etc.

## 📁 Included Files

- `modern-normalize.css`: The stylesheet
- `index.html`: Demo showing its usage and minimal defaults
