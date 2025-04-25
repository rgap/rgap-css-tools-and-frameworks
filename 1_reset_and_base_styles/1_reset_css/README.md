# 📘 Eric Meyer's Reset CSS

## 🕰️ Historical Context

Eric Meyer introduced this reset in the early 2000s (v1), with v2.0 becoming widely adopted by 2011. The purpose was to eliminate inconsistent default browser styles, giving developers a blank, consistent foundation for styling.

- 🔧 Version used here: Reset CSS v2.0 (2011)
- 📖 Source: http://meyerweb.com/eric/tools/css/reset/

## 🎯 Purpose

This reset:

- Removes all default margins and paddings
- Normalizes font sizes and vertical alignments
- Eliminates list styles and quote decorations
- Forces a consistent `border-collapse` on tables
- Sets HTML5 semantic tags to `display: block`

## ⚠️ Criticisms

- **Too aggressive**: removes too much, including useful styles (e.g., `ul` bullets)
- **Extra work**: developers must reapply common styles like lists, headings
- **Not semantic**: treats all elements the same, which goes against purposeful defaults

## ✅ Use Cases

- Useful for **pixel-perfect designs** or CSS from scratch
- Still used in **email templates**, where full control is needed
- Mostly replaced today by **Normalize.css**, **Sanitize.css**, or **Tailwind Preflight**

## 📁 Included Files

- `reset.css`: The original reset stylesheet
- `index.html`: Demo using the reset
