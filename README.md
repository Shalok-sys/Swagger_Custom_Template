# Swagger_Custom_Template
This repository contains the CSS file for a custom swagger theme. Feel free to use it, if you like it !
# 🛠️ Customize Your Own Swagger UI Template

This project provides a basic **Swagger UI** (`basic.html`) integrated with a **custom theme** (`theme-custom.css`). The aim of showing Basic.html file is so that you can get an idea of what classes would be there to modify for improving its CSS. By simply, working on the CSS you can completely change the look of your OpenAPI template. This task is a part of an assignment. Please treat it as such.  
You can easily build your **own customized Swagger interface** by focusing on specific CSS classes without modifying Swagger’s internal JavaScript.

---

## 📁 Project Structure

```plaintext
Below is the usual project strucutre, once you have created a basic working OpenAPI documentation using swagger. 
/
├── basic.html
├── styles/
│   └── theme-custom.css
└── (other assets like favicon, images)
```
Here, you only have to modify them-custom.css ! and your job is done.
---

## 🌟 Key Classes to Customize

| CSS Selector | Purpose | Customization Ideas |
|:-------------|:--------|:--------------------|
| `html, body` | Set global background color and font | Light or dark theme, font family |
| `.topbar` | Top header bar | Change background color (e.g., teal) |
| `.topbar-wrapper .link img` | Logo inside the header | Adjust height, margins |
| `.wrapper`, `.information-container`, `.opblock` | Main content sections and operation cards | Add padding, background color, box shadows |
| `.opblock-summary-method` | HTTP method label (GET, POST, etc.) | Color-code method types |
| `.opblock-summary-path` | API path text | Adjust color and font |
| `.opblock-summary` | Operation block summary | Background, border radius, spacing |
| `.opblock-tag` | API grouping headers (tags like "Maps") | Background color, text styling |
| `button`, `.btn` | All buttons | Set background color, hover transitions |
| `a`, `.link` | Hyperlinks (e.g., API JSON link) | Color and hover effects |
| `input, select, textarea` | Forms and inputs | Styling focus and normal state |
| `.copy-to-clipboard svg`, `.arrow` | Small icons | Adjust icon colors |

---

## 🎨 Styling Ideas

You can apply the following to create a professional Swagger UI:

- **Backgrounds:**  
  ```css
  body {
    background-color: #f7f9fa; /* light background */
  }
  ```

- **Topbar:**
  ```css
  .topbar {
    background-color: #008080; /* teal */
  }
  ```

- **Buttons:**
  ```css
  button, .btn {
    background-color: #008080;
    color: #ffffff;
    border-radius: 5px;
    transition: background-color 0.3s ease;
  }
  button:hover {
    background-color: #cc3366; /* rose on hover */
  }
  ```

- **Cards and Sections:**
  ```css
  .opblock {
    background: #ffffff;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    transition: transform 0.3s ease;
  }
  .opblock:hover {
    transform: translateY(-4px);
  }
  ```

- **Animations:**  [Optional]
  Add soft fade-ins:
  ```css
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(10px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .wrapper, .information-container, .opblock {
    animation: fadeIn 0.6s ease;
  }
  ```

---

## 🚀 How to Customize Your Template

1. Open the file `styles/theme-custom.css`.
2. Focus on the key classes listed above.
3. Adjust colors, paddings, fonts, animations as per your brand/theme.
4. Save changes.
5. Refresh your browser to see the updated Swagger UI.

✅ No need to modify the internal Swagger `swagger-ui.css` or JavaScript!

---

## 📜 Best Practices

- Use **light, consistent color themes** for better readability.
- Keep **animations subtle** to avoid distracting users.
- Prefer **CSS overrides** instead of editing Swagger’s core files for easy upgrades later.
- You can add **custom fonts** via Google Fonts if needed (e.g., `Poppins`, `Inter`, `Roboto`).

Example:
```html
<link href="https://fonts.googleapis.com/css2?family=Inter&display=swap" rel="stylesheet">
```

And then apply:
```css
body {
  font-family: 'Inter', sans-serif;
}
```

---
---
## Results
![image](https://github.com/user-attachments/assets/d9e0d642-7a63-4897-987a-6fa863eb4a5f)

---

## 📢 Notes

- The favicon and Swagger branding (logo) are kept **untouched** for simplicity.
- Feel free to add transitions, dark/light switchers, or advanced animations depending on your project needs.

---

# 🔥 Happy Customizing!

---

