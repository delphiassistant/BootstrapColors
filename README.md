# Bootstrap 5.3 Custom Utilities & Button Library

> **🌐 Live Demo:** [https://delphiassistant.github.io/BootstrapColors](https://delphiassistant.github.io/BootstrapColors)

A comprehensive collection of color utilities and button classes built on Bootstrap 5.3, featuring per-shade color control, stunning hover effects, and production-ready components.

## 📦 What's Included

### 🎨 Color Utilities (`colors.css`)
**495 utility classes** for granular color control:
- 99 text color utilities (`.text-{color}-{shade}`)
- 99 background utilities (`.bg-{color}-{shade}`)
- 99 border color utilities (`.border-{color}-{shade}`)
- 99 auto-contrast chip utilities (`.text-bg-{color}-{shade}`)
- 99 outline chip utilities (`.text-outline-{color}-{shade}`)

### 🔘 Button Classes (`buttons.css`)
**88 button variants** with 8 distinct styles:
- 11 solid buttons (`.btn-{color}`)
- 11 outline buttons (`.btn-outline-{color}`)
- 11 soft buttons (`.btn-soft-{color}`)
- 11 hover effect buttons (`.btn-hover-{color}`)
- 11 glow effect buttons (`.btn-glow-{color}`)
- 11 gradient buttons (`.btn-gradient-{color}`)
- 11 3D effect buttons (`.btn-3d-{color}`)
- 11 bounce effect buttons (`.btn-bounce-{color}`)

---

## 🚀 Quick Start

### Installation

```bash
# Install dependencies
npm install

# Build all CSS
npm run build:css

# Or build individually
npm run build:colors   # Build color utilities
npm run build:buttons  # Build button classes
npm run build:bs       # Build Bootstrap (optional)

# Watch mode (auto-compile on save)
npm run watch:css
```

### Include in Your Project

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Bootstrap CSS (compiled or CDN) -->
  <link rel="stylesheet" href="./css/bootstrap.css" />
  
  <!-- Custom color utilities -->
  <link rel="stylesheet" href="./css/colors.css" />
  
  <!-- Button classes -->
  <link rel="stylesheet" href="./css/buttons.css" />
</head>
<body>
  <!-- Your content here -->
</body>
</html>
```

---

## 🎨 Color Utilities

### Basic Usage

```html
<!-- Text colors -->
<p class="text-blue-600">Blue text</p>
<p class="text-red-700">Red text</p>

<!-- Backgrounds -->
<div class="bg-indigo-200">Light indigo background</div>
<div class="bg-green-800">Dark green background</div>

<!-- Borders -->
<div class="border border-purple-500">Purple border</div>

<!-- Auto-contrast chips -->
<span class="text-bg-blue-500">Blue chip (white text)</span>
<span class="text-bg-yellow-200">Yellow chip (black text)</span>
```

### Available Colors

`blue`, `indigo`, `purple`, `pink`, `red`, `orange`, `yellow`, `green`, `teal`, `cyan`, `gray`

### Shade Range

`100` (lightest) → `200` → `300` → `400` → `500` (base) → `600` → `700` → `800` → `900` (darkest)

📖 **[Read the complete Colors Guide →](COLORS-GUIDE.md)**

---

## 🔘 Button Classes

### Basic Styles

```html
<!-- Solid buttons -->
<button class="btn btn-blue">Blue Button</button>
<button class="btn btn-green">Green Button</button>

<!-- Outline buttons -->
<button class="btn btn-outline-purple">Purple Outline</button>

<!-- Soft buttons -->
<button class="btn btn-soft-pink">Pink Soft</button>
```

### Hover Effect Buttons ✨

```html
<!-- Enhanced hover with ripple -->
<button class="btn btn-hover-blue">Hover Effect</button>

<!-- Pulsing glow -->
<button class="btn btn-glow-red">Glow Effect</button>

<!-- Gradient shift -->
<button class="btn btn-gradient-purple">Gradient</button>

<!-- 3D push-down -->
<button class="btn btn-3d-green">3D Effect</button>

<!-- Bouncy animation -->
<button class="btn btn-bounce-pink">Bounce</button>
```

### Size Variants

```html
<button class="btn btn-lg btn-blue">Large</button>
<button class="btn btn-blue">Default</button>
<button class="btn btn-sm btn-blue">Small</button>
```

📖 **[Read the complete Button Guide →](BUTTON-CLASSES.md)**  
📖 **[Read the Hover Effects Guide →](HOVER-EFFECTS-GUIDE.md)**

---

## 🎬 Interactive Demos

Open these files in your browser to see everything in action:

1. **`demo-colors.html`** - Color utility showcase
   - All 99 color shades
   - Text, background, border, and chip variants
   - Visual color swatches

2. **`demo-standalone-buttons.html`** - Button library showcase
   - Solid, outline, and soft button styles
   - All 11 colors
   - Size variations and practical examples

3. **`demo-hover-effects.html`** - Hover effects showcase
   - All 5 hover animation styles
   - Interactive demonstrations
   - Use case comparisons

4. **`demo-buttons.html`** - Utility-based button examples
   - Manual button construction using utilities
   - Comprehensive color combinations

---

## 📚 Documentation

| Document | Description |
|----------|-------------|
| **[COLORS-GUIDE.md](COLORS-GUIDE.md)** | Complete guide to color utilities |
| **[BUTTON-CLASSES.md](BUTTON-CLASSES.md)** | Complete guide to button classes |
| **[HOVER-EFFECTS-GUIDE.md](HOVER-EFFECTS-GUIDE.md)** | Guide to hover effect animations |

---

## 📁 Project Structure

```
.
├── src/
│   └── scss/
│       ├── colors.scss       # Color utilities source
│       ├── buttons.scss      # Button classes source
│       └── bootstrap.scss    # Bootstrap with customization
├── public/
│   ├── css/
│   │   ├── colors.css        # Compiled color utilities
│   │   ├── buttons.css       # Compiled button classes
│   │   └── bootstrap.css     # Compiled Bootstrap
│   ├── demo-colors.html      # Color utilities demo
│   ├── demo-standalone-buttons.html  # Button classes demo
│   ├── demo-hover-effects.html       # Hover effects demo
│   └── demo-buttons.html     # Utility-based buttons demo
├── node_modules/
│   └── bootstrap/            # Bootstrap 5.3 source
├── package.json              # Build scripts
├── COLORS-GUIDE.md          # Color utilities documentation
├── BUTTON-CLASSES.md        # Button classes documentation
├── HOVER-EFFECTS-GUIDE.md   # Hover effects documentation
└── README.md                # This file
```

---

## 🛠️ Build Scripts

```json
{
  "scripts": {
    "build:bs": "Build Bootstrap CSS",
    "build:colors": "Build color utilities",
    "build:buttons": "Build button classes",
    "build:css": "Build colors + buttons",
    "watch:css": "Watch and auto-compile on changes"
  }
}
```

---

## ✨ Features

### Color Utilities
✅ 99 unique color shades (11 colors × 9 shades)  
✅ 495 total utility classes  
✅ Auto-contrast text for chips  
✅ Bootstrap 5.3 official colors  
✅ Additive (doesn't override Bootstrap)  

### Button Classes
✅ 88 button variants (11 colors × 8 styles)  
✅ Built-in shadows and animations  
✅ Auto-contrast text colors  
✅ Hover, focus, active, disabled states  
✅ 5 unique hover effect animations  
✅ Compatible with Bootstrap sizing  
✅ Production-ready and tested  

### General
✅ Pure CSS (no JavaScript required)  
✅ Hardware-accelerated animations  
✅ Fully accessible (WCAG compliant)  
✅ Responsive and mobile-friendly  
✅ Cross-browser compatible  
✅ English comments throughout  

---

## 🎨 Color Palette

All utilities and buttons use these 11 color families from Bootstrap 5.3:

| Color | Light (200) | Base (500) | Dark (700) |
|-------|-------------|------------|------------|
| **Blue** | `rgb(158, 197, 254)` | `#0d6efd` | `rgb(8, 66, 152)` |
| **Indigo** | `rgb(194, 159, 250)` | `#6610f2` | `rgb(61, 10, 145)` |
| **Purple** | `rgb(197, 179, 230)` | `#6f42c1` | `rgb(67, 40, 116)` |
| **Pink** | `rgb(239, 173, 206)` | `#d63384` | `rgb(128, 31, 79)` |
| **Red** | `rgb(241, 174, 181)` | `#dc3545` | `rgb(132, 32, 41)` |
| **Orange** | `rgb(254, 203, 161)` | `#fd7e14` | `rgb(152, 76, 12)` |
| **Yellow** | `rgb(255, 230, 156)` | `#ffc107` | `rgb(153, 116, 4)` |
| **Green** | `rgb(163, 207, 187)` | `#198754` | `rgb(15, 81, 50)` |
| **Teal** | `rgb(166, 233, 213)` | `#20c997` | `rgb(19, 121, 91)` |
| **Cyan** | `rgb(158, 234, 249)` | `#0dcaf0` | `rgb(8, 121, 144)` |
| **Gray** | `#e9ecef` | `#adb5bd` | `#495057` |

---

## 🎯 Use Cases

### E-commerce
```html
<!-- Product card -->
<div class="card">
  <span class="text-bg-red-500 position-absolute top-0 end-0 m-2">Sale!</span>
  <img src="product.jpg" class="card-img-top" />
  <div class="card-body">
    <h5 class="card-title">Product Name</h5>
    <p class="text-gray-600">$99.99</p>
    <button class="btn btn-hover-blue w-100">Add to Cart</button>
  </div>
</div>
```

### Dashboard
```html
<!-- Status cards -->
<div class="row">
  <div class="col-md-3">
    <div class="card bg-green-50 border-green-400">
      <div class="card-body">
        <h6 class="text-green-800">Active Users</h6>
        <h2 class="text-green-600">1,234</h2>
        <span class="text-bg-green-500">+12%</span>
      </div>
    </div>
  </div>
</div>
```

### Forms
```html
<!-- Form with validation -->
<form>
  <div class="mb-3">
    <label class="form-label text-blue-800">Email</label>
    <input type="email" class="form-control border-blue-400" />
  </div>
  <button type="submit" class="btn btn-gradient-blue">Sign Up</button>
  <button type="button" class="btn btn-outline-gray">Cancel</button>
</form>
```

### Alerts
```html
<div class="bg-yellow-100 border border-yellow-400 text-yellow-800 p-3 rounded">
  <strong>Warning:</strong> Your trial expires in 3 days.
  <button class="btn btn-sm btn-glow-yellow ms-2">Upgrade Now</button>
</div>
```

---

## 🌐 Browser Support

✅ **Modern Browsers:**
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

⚠️ **Graceful Degradation:**
- Older browsers get standard styles without animations
- All functionality remains intact

---

## 💡 Tips & Best Practices

### Color Utilities
1. Use **100-300** for light backgrounds
2. Use **700-900** for text on light backgrounds
3. Use **`.text-bg-*`** for automatic text contrast
4. Maintain 4.5:1 contrast ratio for accessibility
5. Be consistent with shade selections

### Button Classes
1. Use **`.btn-hover-*`** for primary CTAs
2. Use **`.btn-glow-*`** for urgent actions
3. Use **`.btn-gradient-*`** for premium features
4. Use **`.btn-3d-*`** for games/interactive apps
5. Use **`.btn-bounce-*`** for fun/casual interfaces

### Performance
1. Include only what you need
2. Minify CSS for production
3. Use CDN for Bootstrap if preferred
4. Animations are hardware-accelerated
5. No JavaScript dependencies

---

## 📊 Statistics

| Metric | Count |
|--------|-------|
| **Total CSS Classes** | 583 |
| **Color Utilities** | 495 |
| **Button Variants** | 88 |
| **Color Families** | 11 |
| **Shade Levels** | 9 |
| **Hover Effects** | 5 |
| **Demo Pages** | 4 |
| **Documentation Pages** | 4 |

---

## 🤝 Contributing

This is a personal project, but feel free to:
- Report issues
- Suggest improvements
- Share your implementations
- Fork and customize for your needs

---

## 📄 License

Built with Bootstrap 5.3 (MIT License)  
Custom utilities and components provided as-is for personal/commercial use

---

## 🙏 Acknowledgments

- **Bootstrap Team** - For the amazing framework
- **Bootstrap 5.3** - Official color system and maps
- **Sass** - For powerful CSS preprocessing

---

## 📞 Support

For questions or issues:
1. Check the documentation files
2. Review the demo pages
3. Inspect the compiled CSS
4. Refer to Bootstrap's official docs

---

## 🎉 Quick Examples

### Complete Button Example
```html
<div class="d-flex gap-2 flex-wrap">
  <button class="btn btn-blue">Standard</button>
  <button class="btn btn-hover-blue">Hover Effect</button>
  <button class="btn btn-glow-blue">Glow</button>
  <button class="btn btn-gradient-blue">Gradient</button>
  <button class="btn btn-3d-blue">3D</button>
  <button class="btn btn-bounce-blue">Bounce</button>
</div>
```

### Complete Color Example
```html
<div class="bg-blue-100 border border-blue-400 p-4 rounded">
  <h3 class="text-blue-900">Section Title</h3>
  <p class="text-blue-700">Content text with good contrast</p>
  <div class="d-flex gap-2 mt-3">
    <span class="text-bg-blue-500">Tag 1</span>
    <span class="text-bg-blue-600">Tag 2</span>
    <span class="text-outline-blue-500">Tag 3</span>
  </div>
</div>
```

---

**🚀 Ready to use in production • Built with ❤️ using Bootstrap 5.3**

For detailed documentation, see:
- [Colors Guide](COLORS-GUIDE.md)
- [Button Classes](BUTTON-CLASSES.md)
- [Hover Effects](HOVER-EFFECTS-GUIDE.md)

