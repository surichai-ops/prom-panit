# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## 📋 Project Overview

**ร้านชำใส่ใจ (Shop with Care)** - Static landing page for a convenience store in Khon Kaen, Thailand.

### Features
- ✅ Store information (name, hours, address, phone)
- ✅ Weekly promotions
- ✅ Google Street View integration
- ✅ 360° interior view
- ✅ Dark green aesthetic (CCTV vibe)
- ✅ Hosted on GitHub Pages

---

## 🛠 Technology Stack

| Component | Technology |
|-----------|-----------|
| Markup | Pure HTML5 |
| Styling | CSS3 with custom properties |
| Language | Thai (lang="th") |
| Maps | Google Maps Street View (embedded iframe) |
| Build System | **None** - Static files only |
| Hosting | GitHub Pages |

---

## 🚀 Development Workflow

### Quick Start
```bash
# Simply open the HTML file in any browser
# No installation or build process required
open index.html
```

### Making Changes
1. **Edit HTML** → [index.html](index.html)
2. **Edit Styles** → [styles.css](styles.css)
3. **Refresh Browser** → See changes immediately

No package manager, bundler, or dev server needed.

---

## 🏗 Architecture

### File Structure
```
web-me/
├── index.html      # Main page with all content sections
├── styles.css      # Global styles with CSS variables
└── assets/         # (To be created) Images and media
    ├── logo.svg
    ├── storefront.jpg
    └── 360/
        └── interior.jpg
```

### HTML Structure ([index.html](index.html))

```
<header>                  # Logo, store name, tagline
<main>
  <section.hero>          # Storefront photo + hours + contact
  <section.map-360>       # Street View iframe + 360° photo
  <section.promos>        # Weekly promotional items
  <section.contact>       # Address and phone with tel: link
</main>
<footer>                  # Copyright notice
```

---

## 🎨 Design System ([styles.css](styles.css))

### Color Palette (CSS Custom Properties)

| Variable | Value | Usage |
|----------|-------|-------|
| `--bg` | `#0b0f0a` | Dark green background |
| `--fg` | `#d8e6d0` | Light text color |
| `--accent` | `#2f7a55` | Green accent for headings |
| `--muted` | `#92a68f` | Secondary/muted text |
| `--grid` | `rgba(45,95,70,0.15)` | Borders and dividers |

### Typography
- **Font Family**: `"Noto Sans Thai", sans-serif`
- **Headings**: Use `--accent` color
- **Body Text**: Use `--fg` color
- **Secondary Text**: Use `--muted` color

### Layout Patterns
- **Hero Section**: CSS Grid with 2 columns (`grid-template-columns: 1fr 1fr`)
- **Spacing**: Consistent 16-20px padding throughout
- **Border Radius**: 8px for images and iframes
- **Borders**: 1px solid using `--grid` variable

---

## 📦 Missing Assets

The following files are referenced but not yet in the repository:

```bash
assets/logo.svg              # Store logo (SVG format)
assets/storefront.jpg        # Storefront exterior photo
assets/360/interior.jpg      # 360° panoramic interior photo
```

**To add assets:**
```bash
mkdir -p assets/360
# Add your image files to the appropriate directories
```

---

## 🗺 Google Maps Configuration

The Street View iframe at [index.html:29-32](index.html#L29-L32) uses a placeholder URL.

**To configure:**
1. Open Google Maps and navigate to the store location
2. Enter Street View mode
3. Copy the panorama URL or extract the `panoid` parameter
4. Replace `YOUR_PANO_ID` in the iframe src:
   ```html
   <iframe src="https://www.google.com/maps/embed?pb=YOUR_PANO_ID"
   ```

---

## 🌏 Language & Localization

- **Primary Language**: Thai (ภาษาไทย)
- **HTML lang attribute**: `lang="th"`
- **Font**: Noto Sans Thai for proper Thai character rendering
- **Content**: All UI text, headings, and content in Thai

When editing content, maintain Thai language consistency throughout.
