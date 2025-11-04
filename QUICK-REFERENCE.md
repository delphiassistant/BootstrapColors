# Quick Reference Card

A cheat sheet for all utilities and button classes.

## 🎨 Color Utilities

### Pattern
```
.text-{color}-{shade}      → Text color
.bg-{color}-{shade}        → Background color
.border-{color}-{shade}    → Border color
.text-bg-{color}-{shade}   → Chip with auto-contrast
.text-outline-{color}-{shade} → Outline chip
```

### Colors
`blue` `indigo` `purple` `pink` `red` `orange` `yellow` `green` `teal` `cyan` `gray`

### Shades
`100` `200` `300` `400` `500` `600` `700` `800` `900`

### Examples
```html
<p class="text-blue-600">Text</p>
<div class="bg-green-200">Background</div>
<div class="border border-red-500">Border</div>
<span class="text-bg-purple-500">Chip</span>
```

---

## 🔘 Button Classes

### Solid Buttons
```html
<button class="btn btn-{color}">Button</button>
```
**Colors:** `blue` `indigo` `purple` `pink` `red` `orange` `yellow` `green` `teal` `cyan` `gray`

### Outline Buttons
```html
<button class="btn btn-outline-{color}">Button</button>
```

### Soft Buttons
```html
<button class="btn btn-soft-{color}">Button</button>
```

### Hover Effect Buttons
```html
<button class="btn btn-hover-{color}">Button</button>
```
**Effect:** Scale + Ripple + Glow

### Glow Effect Buttons
```html
<button class="btn btn-glow-{color}">Button</button>
```
**Effect:** Pulsing Glow

### Gradient Buttons
```html
<button class="btn btn-gradient-{color}">Button</button>
```
**Effect:** Color Shift

### 3D Buttons
```html
<button class="btn btn-3d-{color}">Button</button>
```
**Effect:** Push Down

### Bounce Buttons
```html
<button class="btn btn-bounce-{color}">Button</button>
```
**Effect:** Elastic Bounce

---

## 📏 Size Modifiers

```html
<button class="btn btn-lg btn-blue">Large</button>
<button class="btn btn-blue">Default</button>
<button class="btn btn-sm btn-blue">Small</button>
```

---

## 🎯 Common Patterns

### Status Indicators
```html
<span class="text-bg-green-500">✓ Success</span>
<span class="text-bg-yellow-500">⚠ Warning</span>
<span class="text-bg-red-500">✕ Error</span>
<span class="text-bg-blue-500">ℹ Info</span>
```

### Alert Box
```html
<div class="bg-blue-100 border border-blue-400 text-blue-800 p-3">
  Alert message
</div>
```

### Card with Colored Header
```html
<div class="card">
  <div class="card-header bg-purple-600 text-white">Header</div>
  <div class="card-body">Content</div>
</div>
```

### Form Actions
```html
<button class="btn btn-hover-blue">Submit</button>
<button class="btn btn-outline-gray">Cancel</button>
```

---

## 🎨 Shade Guide

| Shade | Usage | Example |
|-------|-------|---------|
| 100 | Very light background | `bg-blue-100` |
| 200 | Light background | `bg-blue-200` |
| 300 | Subtle accent | `bg-blue-300` |
| 400 | Medium light | `bg-blue-400` |
| 500 | Base color ⭐ | `bg-blue-500` |
| 600 | Medium dark | `text-blue-600` |
| 700 | Dark text | `text-blue-700` |
| 800 | Very dark | `text-blue-800` |
| 900 | Darkest | `text-blue-900` |

---

## 🌈 Color Meanings

| Color | Use For |
|-------|---------|
| **Blue** | Trust, info, primary actions |
| **Green** | Success, confirm, go |
| **Red** | Error, danger, delete |
| **Yellow** | Warning, caution |
| **Purple** | Premium, VIP |
| **Orange** | Action, energy |
| **Indigo** | Authority, professional |
| **Pink** | Creative, friendly |
| **Cyan/Teal** | Modern, fresh |
| **Gray** | Neutral, disabled |

---

## 💡 Contrast Combinations

### Light Backgrounds
```html
<div class="bg-blue-100 text-blue-900">High contrast</div>
<div class="bg-green-200 text-green-800">Good contrast</div>
```

### Dark Backgrounds
```html
<div class="bg-blue-800 text-white">High contrast</div>
<div class="bg-purple-900 text-purple-100">Good contrast</div>
```

---

## 🎯 Button Selection

| Use Case | Button Class |
|----------|--------------|
| Primary CTA | `.btn-hover-blue` |
| Success | `.btn-green` |
| Danger | `.btn-glow-red` |
| Premium | `.btn-gradient-purple` |
| Secondary | `.btn-outline-gray` |
| Subtle | `.btn-soft-blue` |
| Game/Fun | `.btn-3d-green` or `.btn-bounce-pink` |

---

## 📦 Build Commands

```bash
npm run build:colors    # Build color utilities
npm run build:buttons   # Build button classes
npm run build:css       # Build all
npm run watch:css       # Watch mode
```

---

## 📄 Files

| File | Purpose |
|------|---------|
| `colors.css` | Color utility classes |
| `buttons.css` | Button classes |
| `bootstrap.css` | Bootstrap framework |

---

## 🎬 Demos

| Demo | Shows |
|------|-------|
| `demo-colors.html` | Color utilities |
| `demo-standalone-buttons.html` | Button classes |
| `demo-hover-effects.html` | Hover animations |
| `demo-buttons.html` | Utility-based buttons |

---

## 📚 Full Docs

- **[README.md](README.md)** - Project overview
- **[COLORS-GUIDE.md](COLORS-GUIDE.md)** - Color utilities guide
- **[BUTTON-CLASSES.md](BUTTON-CLASSES.md)** - Button classes guide
- **[HOVER-EFFECTS-GUIDE.md](HOVER-EFFECTS-GUIDE.md)** - Hover effects guide

---

## 📊 Quick Stats

- **583** total CSS classes
- **495** color utilities
- **88** button variants
- **11** color families
- **9** shade levels
- **8** button styles
- **5** hover effects

---

**Print this page for quick reference while coding!**

