# 📘 Clean CSS Reset

## 🕰️ Historical Context

As CSS evolved, developers started creating **minimalistic resets**  
instead of full resets like Reset.css or Normalize.css.

Clean resets focus only on the **most important fixes** without removing everything useful.

- No single official creator — it's a community practice.
- Popular from around **2016** onward with the rise of modern browsers.
- 📖 Example: https://www.joshwcomeau.com/css/custom-css-reset/
- 📖 Example: https://piccalil.li/blog/a-modern-css-reset/

## 🎯 Purpose

A clean CSS reset:

- Applies only essential corrections
- Avoids removing useful browser defaults
- Prepares styles for a consistent layout without overkill

## 🆚 Comparison to Reset.css

| Feature                | Reset.css | Clean Reset |
| ---------------------- | --------- | ----------- |
| Removes everything     | ✅        | ❌          |
| Leaves useful defaults | ❌        | ✅          |
| Size                   | Larger    | Tiny        |
| Maintenance needed     | More      | Minimal     |

## ✅ Use Cases

- Lightweight static sites
- Minimalist web apps
- Projects using **utility-first CSS** (like Tailwind)

## 📁 Included Files

- `clean-reset.css`: The minimalist reset stylesheet
- `index.html`: Demo applying the clean reset
