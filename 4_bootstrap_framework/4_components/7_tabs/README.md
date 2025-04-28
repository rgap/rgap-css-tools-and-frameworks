# 📘 Bootstrap Components — Tabs

## 🕰️ Historical Context

Before Bootstrap, implementing tabs required:

- Custom HTML + CSS + JavaScript.
- Managing active/inactive classes manually.
- Handling show/hide animations by hand.

✅ Bootstrap introduced **Tabs** with built-in toggle functionality, animations, and accessibility support.

---

## 📦 How Bootstrap Tabs Work

Tabs are a combination of:

| Purpose             | Class Example  |
| :------------------ | :------------- |
| Tabs container      | `nav nav-tabs` |
| Tab link/button     | `nav-link`     |
| Tab content         | `tab-content`  |
| Individual tab pane | `tab-pane`     |

✅ Each tab uses `data-bs-toggle="tab"` to link to its content.
✅ Content areas switch automatically when a tab is clicked.

---

## 📄 Basic Tabs Example

```html
<ul class="nav nav-tabs" id="myTab" role="tablist">
  <li class="nav-item" role="presentation">
    <button
      class="nav-link active"
      id="home-tab"
      data-bs-toggle="tab"
      data-bs-target="#home"
      type="button"
      role="tab"
      aria-controls="home"
      aria-selected="true"
    >
      Home
    </button>
  </li>
  <li class="nav-item" role="presentation">
    <button
      class="nav-link"
      id="profile-tab"
      data-bs-toggle="tab"
      data-bs-target="#profile"
      type="button"
      role="tab"
      aria-controls="profile"
      aria-selected="false"
    >
      Profile
    </button>
  </li>
</ul>

<div class="tab-content" id="myTabContent">
  <div class="tab-pane fade show active p-3" id="home" role="tabpanel" aria-labelledby="home-tab">Home tab content.</div>
  <div class="tab-pane fade p-3" id="profile" role="tabpanel" aria-labelledby="profile-tab">Profile tab content.</div>
</div>
```

✅ Automatically switches and animates between tabs.

---

## 🔧 How Bootstrap Handles Tabs

- JavaScript manages active tab classes.
- Shows only the currently selected tab-pane.
- Accessibility attributes like `aria-controls` and `aria-selected` are handled.

---

## 💡 Quick Concept

Tabs = **`nav nav-tabs`** + **`nav-link`** + **`tab-content`** + **`tab-pane`** with matching `data-bs-target`.

---

## 💸 Why Bootstrap Tabs Are Useful

- Quick organization of large content into sections.
- No need to write custom JavaScript.
- Clean, consistent look.
- Mobile-friendly and responsive.
