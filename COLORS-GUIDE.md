# Colors Utility Classes Guide

Per-shade utility classes for all Bootstrap 5.3 colors with auto-contrast support.

## 🎨 Overview

The `colors.css` file provides **granular control** over Bootstrap's color system by generating utility classes for every shade (100-900) of every color family. This gives you access to **99 unique color shades** plus specialized utilities.

### What's Included

- ✅ **396 color utilities** (99 shades × 4 types)
  - Text color utilities (`.text-{color}-{shade}`)
  - Background color utilities (`.bg-{color}-{shade}`)
  - Border color utilities (`.border-{color}-{shade}`)
  - Combined text-bg chips (`.text-bg-{color}-{shade}`)
- ✅ **99 outline chip variants** (`.text-outline-{color}-{shade}`)
- ✅ **Auto-contrast text** using Bootstrap's `color-contrast()` function
- ✅ **All Bootstrap color families** (11 colors × 9 shades each)

---

## 🚀 Quick Start

### 1. Include the CSS

```html
<link rel="stylesheet" href="./css/bootstrap.css" />
<link rel="stylesheet" href="./css/colors.css" />
```

### 2. Use the utilities

```html
<!-- Text colors -->
<p class="text-blue-600">Blue text</p>
<p class="text-red-700">Red text</p>

<!-- Backgrounds -->
<div class="bg-indigo-200">Light indigo background</div>
<div class="bg-green-800">Dark green background</div>

<!-- Borders -->
<div class="border border-purple-500">Purple border</div>

<!-- Chips with auto-contrast -->
<span class="text-bg-blue-500">Blue chip</span>
<span class="text-bg-yellow-200">Yellow chip</span>
```

---

## 🎨 Available Colors

All utilities are available for these 11 color families:

| Color | Shades | Example |
|-------|--------|---------|
| **Blue** | 100-900 | `.text-blue-500`, `.bg-blue-300` |
| **Indigo** | 100-900 | `.text-indigo-600`, `.bg-indigo-200` |
| **Purple** | 100-900 | `.text-purple-500`, `.bg-purple-400` |
| **Pink** | 100-900 | `.text-pink-600`, `.bg-pink-300` |
| **Red** | 100-900 | `.text-red-700`, `.bg-red-200` |
| **Orange** | 100-900 | `.text-orange-500`, `.bg-orange-300` |
| **Yellow** | 100-900 | `.text-yellow-600`, `.bg-yellow-200` |
| **Green** | 100-900 | `.text-green-700`, `.bg-green-300` |
| **Teal** | 100-900 | `.text-teal-500`, `.bg-teal-400` |
| **Cyan** | 100-900 | `.text-cyan-600`, `.bg-cyan-200` |
| **Gray** | 100-900 | `.text-600`, `.bg-300` |

### Shade Scale

- **100** - Lightest (10% darkness)
- **200** - Very Light (20% darkness)
- **300** - Light (30% darkness)
- **400** - Medium Light (40% darkness)
- **500** - Base Color (50% - default)
- **600** - Medium Dark (60% darkness)
- **700** - Dark (70% darkness)
- **800** - Very Dark (80% darkness)
- **900** - Darkest (90% darkness)

---

## 📦 Utility Types

### 1. Text Color (`.text-{color}-{shade}`)

Apply color to text content.

```html
<p class="text-blue-500">Base blue text</p>
<p class="text-blue-700">Darker blue text</p>
<p class="text-red-600">Medium dark red text</p>
<h1 class="text-purple-800">Dark purple heading</h1>
```

**Use cases:**
- Headings with custom colors
- Emphasis text
- Links and interactive text
- Status indicators

### 2. Background Color (`.bg-{color}-{shade}`)

Apply background color to elements.

```html
<div class="bg-blue-100">Very light blue background</div>
<div class="bg-green-500">Base green background</div>
<div class="bg-red-900">Very dark red background</div>
```

**Use cases:**
- Colored sections
- Cards and panels
- Alerts and notifications
- Highlight blocks

### 3. Border Color (`.border-{color}-{shade}`)

Apply color to borders. **Note:** Requires Bootstrap's `.border` class.

```html
<div class="border border-blue-500">Blue border</div>
<div class="border border-2 border-red-600">Thick red border</div>
<div class="border-top border-green-700">Green top border</div>
```

**Use cases:**
- Card outlines
- Input field borders
- Dividers
- Decorative borders

### 4. Text-Background Chips (`.text-bg-{color}-{shade}`)

Combined utility with background color and **auto-contrast text**.

```html
<span class="text-bg-blue-500">Blue chip</span>
<span class="text-bg-yellow-200">Yellow chip (auto black text)</span>
<span class="text-bg-purple-800">Purple chip (auto white text)</span>
```

**Features:**
- Automatic text color (white or black) for optimal contrast
- Built-in padding (`.25rem .5rem`)
- Rounded corners (`.25rem`)
- Inline-block display

**Use cases:**
- Tags and badges
- Status indicators
- Category labels
- Pill buttons

### 5. Outline Chips (`.text-outline-{color}-{shade}`)

Transparent background with colored border and text.

```html
<span class="text-outline-blue-500">Outlined chip</span>
<span class="text-outline-green-600">Outlined badge</span>
```

**Features:**
- Transparent background
- Colored border (1px solid)
- Colored text matching border
- Built-in padding and rounded corners

**Use cases:**
- Secondary badges
- Outlined tags
- Ghost-style labels

---

## 💡 Practical Examples

### Status Indicators

```html
<!-- Success states -->
<span class="text-bg-green-100">✓ Completed</span>
<span class="text-bg-green-500">✓ Active</span>
<span class="text-bg-green-700">✓ Verified</span>

<!-- Warning states -->
<span class="text-bg-yellow-200">⚠ Pending</span>
<span class="text-bg-yellow-500">⚠ Review Required</span>

<!-- Error states -->
<span class="text-bg-red-200">✕ Failed</span>
<span class="text-bg-red-600">✕ Critical Error</span>

<!-- Info states -->
<span class="text-bg-blue-200">ℹ Draft</span>
<span class="text-bg-blue-600">ℹ Processing</span>
```

### Category Tags

```html
<span class="text-bg-purple-300">Design</span>
<span class="text-bg-blue-300">Development</span>
<span class="text-bg-green-300">Marketing</span>
<span class="text-bg-orange-300">Sales</span>
<span class="text-bg-pink-300">Support</span>
```

### Priority Levels

```html
<!-- Low priority - light colors -->
<span class="text-bg-gray-200">Low Priority</span>

<!-- Medium priority - medium colors -->
<span class="text-bg-yellow-400">Medium Priority</span>

<!-- High priority - dark colors -->
<span class="text-bg-orange-600">High Priority</span>

<!-- Urgent - very dark colors -->
<span class="text-bg-red-700">Urgent</span>
```

### Alert Messages

```html
<!-- Info alert -->
<div class="bg-blue-100 border-blue-400 text-blue-800 p-3 border rounded">
  <strong>Info:</strong> Your changes have been saved.
</div>

<!-- Success alert -->
<div class="bg-green-100 border-green-400 text-green-800 p-3 border rounded">
  <strong>Success:</strong> Operation completed successfully.
</div>

<!-- Warning alert -->
<div class="bg-yellow-100 border-yellow-400 text-yellow-800 p-3 border rounded">
  <strong>Warning:</strong> Please review your settings.
</div>

<!-- Error alert -->
<div class="bg-red-100 border-red-400 text-red-800 p-3 border rounded">
  <strong>Error:</strong> Something went wrong.
</div>
```

### Cards with Colored Headers

```html
<div class="card">
  <div class="card-header bg-purple-600 text-white">
    Premium Feature
  </div>
  <div class="card-body">
    <p>Access exclusive content and features.</p>
  </div>
</div>

<div class="card">
  <div class="card-header bg-blue-100 text-blue-800 border-blue-300">
    Information
  </div>
  <div class="card-body">
    <p>Important information about your account.</p>
  </div>
</div>
```

### Progress/Severity Indicators

```html
<!-- From light to dark = low to high severity -->
<div class="d-flex gap-2">
  <div class="bg-green-200 p-2 flex-fill">10%</div>
  <div class="bg-green-300 p-2 flex-fill">20%</div>
  <div class="bg-yellow-300 p-2 flex-fill">30%</div>
  <div class="bg-yellow-400 p-2 flex-fill">40%</div>
  <div class="bg-orange-400 p-2 flex-fill">50%</div>
  <div class="bg-orange-500 p-2 flex-fill">60%</div>
  <div class="bg-red-500 p-2 flex-fill">70%</div>
  <div class="bg-red-600 p-2 flex-fill text-white">80%</div>
  <div class="bg-red-700 p-2 flex-fill text-white">90%</div>
  <div class="bg-red-800 p-2 flex-fill text-white">100%</div>
</div>
```

### Text Emphasis

```html
<p>
  This is regular text with 
  <span class="text-blue-600">highlighted blue text</span> and 
  <span class="text-red-600">important red text</span>.
</p>

<h2 class="text-purple-700">Section Heading</h2>
<p class="text-gray-600">Supporting text in gray</p>
```

---

## 🎨 Color Combinations

### Light Backgrounds with Dark Text

```html
<div class="bg-blue-100 text-blue-900 p-3">
  Light blue background with dark blue text
</div>

<div class="bg-green-200 text-green-900 p-3">
  Light green background with dark green text
</div>

<div class="bg-yellow-100 text-yellow-900 p-3">
  Light yellow background with dark yellow text
</div>
```

### Dark Backgrounds with Light Text

```html
<div class="bg-blue-800 text-blue-100 p-3">
  Dark blue background with light blue text
</div>

<div class="bg-purple-900 text-purple-100 p-3">
  Very dark purple background with light purple text
</div>
```

### Bordered Elements

```html
<div class="border border-2 border-indigo-500 bg-indigo-50 text-indigo-700 p-3">
  Indigo-themed bordered box
</div>

<div class="border-start border-4 border-red-600 bg-red-50 text-red-800 p-3">
  Left-bordered alert style
</div>
```

---

## 🎯 Shade Selection Guide

### For Backgrounds

| Shade | Use Case | Text Color |
|-------|----------|------------|
| 100-200 | Subtle highlights, hover states | Dark (700-900) |
| 300-400 | Light sections, secondary areas | Medium-Dark (600-800) |
| 500-600 | Prominent sections, primary areas | White or 100-200 |
| 700-900 | Headers, footers, dark themes | White or 100 |

### For Text

| Shade | Use Case | Best On |
|-------|----------|---------|
| 100-300 | Light text on dark backgrounds | Dark BG (700-900) |
| 400-600 | Medium contrast text | Any light BG |
| 700-900 | High contrast text, primary text | White or light BG |

### For Borders

| Shade | Use Case |
|-------|----------|
| 200-400 | Subtle dividers, light borders |
| 500-600 | Standard borders, card outlines |
| 700-900 | Prominent borders, emphasis |

---

## 🌈 Color Psychology & Usage

### Blue (`blue-*`)
**Meaning:** Trust, reliability, professionalism  
**Use for:** Corporate content, tech products, trust indicators

```html
<span class="text-bg-blue-500">Verified</span>
<div class="bg-blue-100 text-blue-800 p-3">Information panel</div>
```

### Green (`green-*`)
**Meaning:** Success, growth, confirmation  
**Use for:** Success messages, confirmations, go-ahead actions

```html
<span class="text-bg-green-500">✓ Success</span>
<div class="bg-green-100 text-green-800 p-3">Success message</div>
```

### Red (`red-*`)
**Meaning:** Danger, error, stop  
**Use for:** Errors, warnings, delete actions

```html
<span class="text-bg-red-600">✕ Error</span>
<div class="bg-red-100 text-red-800 p-3">Error message</div>
```

### Yellow (`yellow-*`)
**Meaning:** Warning, caution, attention  
**Use for:** Warnings, important notices, pending states

```html
<span class="text-bg-yellow-500">⚠ Warning</span>
<div class="bg-yellow-100 text-yellow-800 p-3">Warning message</div>
```

### Purple (`purple-*`)
**Meaning:** Premium, luxury, creativity  
**Use for:** Premium features, VIP content, creative sections

```html
<span class="text-bg-purple-600">Premium</span>
<div class="bg-purple-100 text-purple-800 p-3">VIP feature</div>
```

### Orange (`orange-*`)
**Meaning:** Energy, enthusiasm, action  
**Use for:** CTAs, important updates, featured content

```html
<span class="text-bg-orange-500">New!</span>
<div class="bg-orange-100 text-orange-800 p-3">Featured</div>
```

### Cyan/Teal (`cyan-*`, `teal-*`)
**Meaning:** Modern, fresh, digital  
**Use for:** Tech features, modern UI, informational content

```html
<span class="text-bg-cyan-500">Beta</span>
<span class="text-bg-teal-500">New Feature</span>
```

### Pink (`pink-*`)
**Meaning:** Creative, friendly, approachable  
**Use for:** Creative content, social features, friendly actions

```html
<span class="text-bg-pink-500">Featured</span>
<div class="bg-pink-100 text-pink-800 p-3">Community post</div>
```

### Indigo (`indigo-*`)
**Meaning:** Authority, sophistication, depth  
**Use for:** Professional content, authority indicators

```html
<span class="text-bg-indigo-600">Expert</span>
<div class="bg-indigo-100 text-indigo-800 p-3">Pro tip</div>
```

### Gray (`gray-*` or just numbers)
**Meaning:** Neutral, professional, subtle  
**Use for:** Disabled states, secondary content, backgrounds

```html
<span class="text-bg-600">Inactive</span>
<div class="bg-200 text-700 p-3">Neutral section</div>
```

---

## 🎨 Design Patterns

### Monochromatic Design

Use multiple shades of the same color:

```html
<div class="bg-blue-100 p-4">
  <h3 class="text-blue-900">Section Title</h3>
  <p class="text-blue-700">Main content text</p>
  <div class="bg-blue-200 border border-blue-400 text-blue-800 p-3 mt-3">
    Highlighted box
  </div>
  <button class="btn bg-blue-600 border-blue-600 text-white mt-3">
    Action Button
  </button>
</div>
```

### Complementary Colors

Combine complementary colors for contrast:

```html
<!-- Blue + Orange -->
<div class="bg-blue-600 text-white p-3">
  <span class="text-bg-orange-500">Hot!</span> Special Offer
</div>

<!-- Purple + Yellow -->
<div class="bg-purple-100 border border-purple-400 p-3">
  <span class="text-bg-yellow-400">New</span>
  <span class="text-purple-900">Feature Released</span>
</div>
```

### Analogous Colors

Use adjacent colors on the color wheel:

```html
<!-- Blue → Indigo → Purple -->
<div class="d-flex gap-2">
  <span class="text-bg-blue-500">Tag 1</span>
  <span class="text-bg-indigo-500">Tag 2</span>
  <span class="text-bg-purple-500">Tag 3</span>
</div>
```

---

## 💻 Code Examples

### Dashboard Status Cards

```html
<div class="row">
  <div class="col-md-3">
    <div class="card border-green-400">
      <div class="card-body bg-green-50">
        <h5 class="text-green-800">Total Sales</h5>
        <p class="text-green-600 fs-2 mb-0">$45,230</p>
        <span class="text-bg-green-500 mt-2">+12%</span>
      </div>
    </div>
  </div>
  
  <div class="col-md-3">
    <div class="card border-blue-400">
      <div class="card-body bg-blue-50">
        <h5 class="text-blue-800">New Users</h5>
        <p class="text-blue-600 fs-2 mb-0">1,234</p>
        <span class="text-bg-blue-500 mt-2">+8%</span>
      </div>
    </div>
  </div>
</div>
```

### Multi-level Tags

```html
<!-- Priority tags -->
<span class="text-bg-red-700">Critical</span>
<span class="text-bg-orange-600">High</span>
<span class="text-bg-yellow-500">Medium</span>
<span class="text-bg-blue-400">Low</span>
<span class="text-bg-gray-300">None</span>
```

### Sidebar Navigation

```html
<div class="bg-indigo-900 text-white p-3">
  <h5 class="text-indigo-100">Menu</h5>
  <ul class="nav flex-column">
    <li class="nav-item">
      <a href="#" class="nav-link text-white bg-indigo-800">Dashboard</a>
    </li>
    <li class="nav-item">
      <a href="#" class="nav-link text-indigo-200">Reports</a>
    </li>
    <li class="nav-item">
      <a href="#" class="nav-link text-indigo-200">Settings</a>
    </li>
  </ul>
</div>
```

---

## 🔧 Customization Tips

### Hover States

Combine with `:hover` for interactive elements:

```html
<style>
.hover-bg-blue:hover {
  background-color: rgb(158.2, 197, 254.2) !important; /* blue-200 */
}
</style>

<button class="btn bg-blue-100 text-blue-800 hover-bg-blue">
  Hover Me
</button>
```

### Responsive Colors

Use Bootstrap responsive utilities:

```html
<div class="bg-blue-200 bg-md-blue-400 bg-lg-blue-600 p-3">
  <!-- Note: You may need to create responsive variants -->
  Different colors at different breakpoints
</div>
```

---

## 📊 All Available Classes

### Summary

| Utility Type | Pattern | Count | Example |
|--------------|---------|-------|---------|
| Text | `.text-{color}-{shade}` | 99 | `.text-blue-600` |
| Background | `.bg-{color}-{shade}` | 99 | `.bg-green-300` |
| Border | `.border-{color}-{shade}` | 99 | `.border-red-500` |
| Text-BG Chip | `.text-bg-{color}-{shade}` | 99 | `.text-bg-purple-400` |
| Outline Chip | `.text-outline-{color}-{shade}` | 99 | `.text-outline-cyan-600` |
| **Total** | | **495** | |

---

## 🎯 Best Practices

### DO ✅

1. **Use meaningful shades** - 100-300 for backgrounds, 700-900 for text
2. **Maintain contrast** - Ensure text is readable on backgrounds (4.5:1 ratio)
3. **Be consistent** - Use same shade levels across your design
4. **Use `.text-bg-*`** - For chips/badges to get automatic contrast
5. **Combine wisely** - Light background + dark text, or vice versa

### DON'T ❌

1. **Don't use random shades** - Pick a system (e.g., always use 100, 500, 700)
2. **Don't sacrifice contrast** - Avoid `text-blue-500` on `bg-blue-400`
3. **Don't overuse colors** - Stick to 2-3 main colors per section
4. **Don't ignore accessibility** - Test with color contrast checkers
5. **Don't forget hover states** - Interactive elements need clear feedback

---

## ♿ Accessibility

### Contrast Guidelines (WCAG)

- **AA Standard:** 4.5:1 contrast ratio for normal text
- **AAA Standard:** 7:1 contrast ratio for normal text
- **Large Text:** 3:1 contrast ratio (18pt+ or 14pt+ bold)

### Recommended Combinations

**High Contrast (AAA):**
```html
<p class="text-blue-900 bg-blue-100">Excellent contrast</p>
<p class="text-white bg-blue-800">Excellent contrast</p>
```

**Good Contrast (AA):**
```html
<p class="text-blue-800 bg-blue-200">Good contrast</p>
<p class="text-white bg-blue-600">Good contrast</p>
```

**Avoid (Poor Contrast):**
```html
<p class="text-blue-400 bg-blue-300">⚠️ Poor contrast</p>
<p class="text-blue-600 bg-blue-500">⚠️ Poor contrast</p>
```

---

## 🎬 Demo

View all color utilities in action:
👉 **Open `demo-colors.html`** to see interactive color swatches

---

## 📦 Build Information

**Source:** `src/scss/colors.scss`  
**Compiled:** `public/css/colors.css`  
**Build command:** `npm run build:colors`

**Based on:** Bootstrap 5.3 official color maps  
**Auto-contrast:** Using Bootstrap's `color-contrast()` function  
**Additive:** Does not override Bootstrap's own utilities

---

## 🔗 Related Resources

- **Button Classes:** See `BUTTON-CLASSES.md`
- **Hover Effects:** See `HOVER-EFFECTS-GUIDE.md`
- **Bootstrap Docs:** [Bootstrap Colors](https://getbootstrap.com/docs/5.3/customize/color/)

---

**Built with ❤️ using Bootstrap 5.3 Sass**

