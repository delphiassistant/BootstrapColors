# Standalone Button Classes

Beautiful, ready-to-use button classes with built-in shadows, smooth animations, and stunning hover effects.

## 🚀 Quick Start

### 1. Include the CSS files

```html
<link rel="stylesheet" href="./css/bootstrap.css" />
<link rel="stylesheet" href="./css/buttons.css" />
```

### 2. Use the button classes

```html
<!-- Solid buttons -->
<button class="btn btn-blue">Blue Button</button>
<button class="btn btn-green">Green Button</button>

<!-- Outline buttons -->
<button class="btn btn-outline-purple">Purple Outline</button>

<!-- Soft buttons (light background) -->
<button class="btn btn-soft-pink">Pink Soft</button>
```

## 🎨 Available Colors

All buttons are available in 11 colors:
- `blue`
- `indigo`
- `purple`
- `pink`
- `red`
- `orange`
- `yellow`
- `green`
- `teal`
- `cyan`
- `gray`

## 📦 Button Styles

### 1. Solid Buttons (`.btn-{color}`)
Bold, colorful buttons with shadows and hover effects.

```html
<button class="btn btn-blue">Click Me</button>
<button class="btn btn-green">Submit</button>
<button class="btn btn-red">Delete</button>
```

**Features:**
- Auto-contrast text color (white or black)
- Multi-layer shadow for depth
- Smooth hover animation (lift effect)
- Darker shade on hover
- Focus ring support
- Active state feedback
- Disabled state support

### 2. Outline Buttons (`.btn-outline-{color}`)
Transparent background with colored border.

```html
<button class="btn btn-outline-blue">Outlined</button>
<button class="btn btn-outline-green">Secondary</button>
```

**Features:**
- Transparent background
- Colored border and text
- Fills with color on hover
- Subtle shadow
- Perfect for secondary actions

### 3. Soft Buttons (`.btn-soft-{color}`)
Light background with colored text (subtle style).

```html
<button class="btn btn-soft-blue">Soft Blue</button>
<button class="btn btn-soft-green">Soft Green</button>
```

**Features:**
- Light tinted background (10% opacity)
- Darker colored text
- Minimal shadow
- Great for status indicators
- Ideal for less prominent actions

### 4. Hover Effect Buttons (`.btn-hover-{color}`)
Enhanced hover with scale, glow, and ripple animation.

```html
<button class="btn btn-hover-blue">Hover Effect</button>
<button class="btn btn-hover-purple">Enhanced</button>
```

**Features:**
- Scales to 105% on hover
- Ripple effect from center
- Enhanced multi-layer shadow
- Outer ring glow effect
- Perfect for primary CTAs

### 5. Glow Effect Buttons (`.btn-glow-{color}`)
Pulsing glow animation for attention-grabbing buttons.

```html
<button class="btn btn-glow-red">Urgent Action</button>
<button class="btn btn-glow-green">Success</button>
```

**Features:**
- Continuous pulsing glow (1.5s cycle)
- Multi-layer halo effect
- Great for alerts and urgent actions
- Eye-catching without being distracting

### 6. Gradient Effect Buttons (`.btn-gradient-{color}`)
Smooth gradient shift animation.

```html
<button class="btn btn-gradient-purple">Premium</button>
<button class="btn btn-gradient-indigo">Gradient</button>
```

**Features:**
- Diagonal gradient (light to dark)
- Smooth color transition on hover
- Sophisticated premium look
- Perfect for upgrade buttons

### 7. 3D Effect Buttons (`.btn-3d-{color}`)
Physical push-down effect with realistic depth.

```html
<button class="btn btn-3d-green">Push Me</button>
<button class="btn btn-3d-blue">3D Button</button>
```

**Features:**
- Raised appearance with shadow
- Pushes down 2px on hover
- Pushes down 5px on click
- Realistic tactile feedback
- Great for games and interactive apps

### 8. Bounce Effect Buttons (`.btn-bounce-{color}`)
Playful bouncing animation with elastic easing.

```html
<button class="btn btn-bounce-pink">Bouncy</button>
<button class="btn btn-bounce-yellow">Fun!</button>
```

**Features:**
- Scales to 110% with bounce
- Elastic easing for playful feel
- Bounces up to 115% at peak
- Perfect for casual apps and children's interfaces

## 🎭 Button States

All buttons automatically support:

### Hover State
```html
<!-- Hover to see lift animation and color change -->
<button class="btn btn-purple">Hover Me</button>
```

### Active State
```html
<!-- Click to see pressed effect -->
<button class="btn btn-blue">Click Me</button>
```

### Focus State
```html
<!-- Tab to focus and see ring -->
<button class="btn btn-green">Focus Me</button>
```

### Disabled State
```html
<button class="btn btn-red" disabled>Disabled</button>
<button class="btn btn-outline-blue" disabled>Disabled</button>
```

## 📏 Size Variants

Combine with Bootstrap size classes:

```html
<!-- Large -->
<button class="btn btn-lg btn-blue">Large Button</button>

<!-- Default -->
<button class="btn btn-blue">Default Button</button>

<!-- Small -->
<button class="btn btn-sm btn-blue">Small Button</button>
```

## 💡 Practical Examples

### Form Actions
```html
<button class="btn btn-blue">Save Changes</button>
<button class="btn btn-outline-gray">Cancel</button>
```

### CRUD Operations
```html
<button class="btn btn-green">Create</button>
<button class="btn btn-blue">Update</button>
<button class="btn btn-red">Delete</button>
<button class="btn btn-soft-gray">View</button>
```

### Status Buttons
```html
<button class="btn btn-soft-green">✓ Approved</button>
<button class="btn btn-soft-yellow">⏳ Pending</button>
<button class="btn btn-soft-red">✕ Rejected</button>
```

### With Icons
```html
<button class="btn btn-blue">
  <svg>...</svg> Save
</button>
<button class="btn btn-green">
  ✓ Confirm
</button>
```

### Button Groups
```html
<div class="btn-group">
  <button class="btn btn-blue">Day</button>
  <button class="btn btn-outline-blue">Week</button>
  <button class="btn btn-outline-blue">Month</button>
</div>
```

## 🎨 Shadow System

### Solid Buttons
- **Default**: 2-layer shadow (4px + 2px blur)
- **Hover**: Enhanced 2-layer shadow (15px + 6px blur) + lift
- **Active**: Reduced shadow (pressed effect)
- **Focus**: Ring shadow + base shadow

### Outline Buttons
- **Default**: Subtle 1-layer shadow
- **Hover**: Enhanced shadow + lift + color fill

### Soft Buttons
- **Default**: Minimal shadow (1px blur)
- **Hover**: Medium shadow (6px blur) + lift

## 🛠️ Build Commands

```bash
# Build button classes
npm run build:buttons

# Build all CSS (colors + buttons)
npm run build:css

# Watch mode (auto-compile on save)
npm run watch:css
```

## 📊 Total Classes Generated

- **88 button variants** (11 colors × 8 styles)
  - 11 solid buttons
  - 11 outline buttons
  - 11 soft buttons
  - 11 hover effect buttons
  - 11 glow effect buttons
  - 11 gradient buttons
  - 11 3D buttons
  - 11 bounce buttons
- **All with hover, active, focus, and disabled states**
- **Compatible with Bootstrap sizing utilities**

## ✨ Features

✅ **Auto-contrast text** - Automatically chooses black or white text  
✅ **Built-in shadows** - Beautiful depth with multi-layer shadows  
✅ **Smooth animations** - 200ms transitions for all states  
✅ **Hover lift effect** - Buttons lift up 1-2px on hover  
✅ **Focus rings** - Accessible focus indicators  
✅ **Disabled support** - Proper disabled state styling  
✅ **Bootstrap compatible** - Works with all Bootstrap utilities  
✅ **Production ready** - Optimized and tested  

## 🎯 Demo Files

- **`demo-hover-effects.html`** - ⭐ NEW! Showcase of all 5 hover effect styles
- **`demo-standalone-buttons.html`** - Complete showcase of solid, outline, and soft buttons
- **`demo-buttons.html`** - Original utility-based buttons demo
- **`demo-colors.html`** - Color utility classes demo

## 📝 Source Files

- **`src/scss/buttons.scss`** - Button classes source
- **`public/css/buttons.css`** - Compiled button styles

---

**Built with Bootstrap 5.3** • **Uses official color maps** • **Fully responsive**

