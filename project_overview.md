# 📋 Project Overview — Creative Agency Landing Page

## 🎯 Goal
Build a visually appealing **agency landing page** using hand-written HTML and CSS, without any frameworks, focusing on layout composition, typography, and card design.

## 📄 HTML Structure
```
body
└── div.main
    ├── img.logo
    ├── h1  "We are a <span class='creative'>Creative</span> Design Agency"
    ├── div.left.card
    │   ├── img.tile-image
    │   ├── h2.card-title  "Beauty"
    │   └── p.card-text
    └── div.right.card
        ├── img.tile-image
        ├── h2.card-title  "Construction"
        └── p
footer
└── p  "Create. Develop. Design."
```

## 🧠 CSS Layout Strategy

### Two-Column Card Layout
The `.main` container needs to be laid out so `.left.card` and `.right.card` appear side by side. The recommended approach is Flexbox:
```css
.main {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  padding: 40px;
}
.card {
  flex: 1;
  min-width: 300px;
}
```

### The "Creative" Accent Color
The `<span class="creative">` wraps the word "Creative" in the heading. You can style it with:
```css
.creative {
  color: #e74c3c;   /* or any accent color */
}
```

### Google Fonts Integration
Poppins is imported in `<head>` via CDN links. Apply it as:
```css
body {
  font-family: 'Poppins', sans-serif;
}
```

## 📊 Difficulty Level
| Aspect | Rating |
|---|---|
| HTML | ⭐⭐ (simple, clean structure) |
| CSS | ⭐⭐ (Flexbox layout, font, basic styling) |
| JavaScript | ⭐ (none) |
| Overall | ⭐⭐ Beginner-Friendly |

## 💡 Next Steps
- Add hover effects to the cards (scale transform, box-shadow)
- Make it fully responsive with `@media` queries
- Add a navigation bar at the top
- Add an animated typing effect to the hero heading
- Add a contact form section
