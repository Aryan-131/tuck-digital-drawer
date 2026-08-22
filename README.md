# TUCK — Landing Page

A fictional digital organizer product landing page. TUCK is a "digital drawer" for saving and organizing things like links, screenshots, receipts, notes, PDFs, and more.

**Tagline:** "Keep the things you don't want to lose."

---

## Project Overview

This is a responsive, single-page landing page built to demonstrate:

- Clean, editorial design
- Responsive web design (mobile-first)
- Semantic HTML5
- CSS Grid and Flexbox
- Vanilla JavaScript
- Thoughtful UX and micro-interactions
- Accessibility best practices

## Design Philosophy

TUCK is designed to feel:
- **Warm** — Off-white, muted palette
- **Editorial** — Serif display headings, elegant typography
- **Tactile** — Paper-like elements, natural composition
- **Human** — Simple language, no corporate jargon
- **Minimal** — Whitespace, purpose-driven elements

NOT:
- SaaS dashboard aesthetic
- Dark theme / developer-focused
- AI-generated template
- Overly rounded or neon-colored UI

---

## Color Palette

| Color | Value | Usage |
|-------|-------|-------|
| Background | `#F5F1E8` | Primary page background |
| Surface | `#FFFDF8` | Cards, components |
| Primary Text | `#252525` | Headings, body text |
| Secondary Text | `#77736C` | Supporting text, muted |
| Primary Accent | `#E36A3D` | Orange highlights, CTAs |
| Secondary Accent | `#7A8467` | Green alternative accent |
| Soft Surface | `#E8E0D2` | Subtle backgrounds |
| Border | `#D9D1C3` | Lines, dividers |

---

## Typography

**Headings:** DM Serif Display (serif, editorial feel)
**Body:** Inter (clean, modern sans-serif)

Typography uses `clamp()` for fluid scaling:
- Hero heading: 2.5rem → 4rem
- Section headings: 2rem → 3.5rem
- Body text: 16px default

---

## Responsive Breakpoints

- **Desktop:** 1200px+
- **Laptop:** 1024px–1199px
- **Tablet:** 768px–1023px
- **Mobile:** 480px–767px
- **Small mobile:** 320px–479px

Mobile navigation becomes a hamburger menu at ~834px.

---

## File Structure

```
tuck/
├── index.html              # Main HTML
├── css/
│   ├── style.css           # Base styles, layout, components
│   └── responsive.css      # Media queries for all breakpoints
├── js/
│   └── script.js           # Navigation, interactions, smooth scroll
├── assets/
│   ├── images/             # Placeholder for images (not included)
│   └── icons/              # Placeholder for icons (not included)
└── README.md
```

---

## Sections

### 1. **Hero** 
Two-column layout (desktop) with heading, description, CTAs, and a visual representation of saved items (screenshots, links, receipts, etc.)

### 2. **Problem**
Shows the pain point: things are saved everywhere (gallery, chat, downloads, messages) and hard to find later.

### 3. **How It Works**
Three steps: Save It → Tuck It Away → Find It Later. Editorial layout with large numbers.

### 4. **Product Preview**
A realistic interface mockup showing the Tuck app with:
- Sidebar navigation (collections)
- Search bar
- Grid of saved items

### 5. **Collections**
Masonry grid of collection cards (Trips, Shopping, College, Ideas, Recipes, Work) with varied sizes.

### 6. **Search Experience**
Demonstrates the key benefit: search by what you remember, not where you saved it.

### 7. **Final CTA**
Large editorial statement with primary and secondary buttons.

### 8. **Footer**
Minimal footer with brand, links, social icons, and copyright.

---

## Features

- ✅ **Responsive Design** — Works on all device sizes
- ✅ **Smooth Scrolling** — Anchor link navigation
- ✅ **Mobile Navigation** — Hamburger menu on small screens
- ✅ **Fade-in Animations** — Subtle reveal effects with Intersection Observer
- ✅ **Hover Effects** — Micro-interactions on cards and buttons
- ✅ **Accessibility** — Semantic HTML, ARIA labels, keyboard navigation
- ✅ **Performance** — No external dependencies, minimal JavaScript
- ✅ **SEO-friendly** — Proper meta tags, semantic structure

---

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Android)
- ES6+ JavaScript (no IE11 support, by design)

---

## Running the Project

1. **Clone or download** the project
2. **Open `index.html`** in a web browser
3. Or serve locally:
   ```bash
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

No build tools or dependencies required.

---

## JavaScript Usage

- **Mobile Menu:** Toggle on hamburger click
- **Smooth Scroll:** Anchor links navigate smoothly
- **Animations:** Intersection Observer triggers fade-in on scroll
- **Search Demo:** Visual feedback on input focus
- **Sidebar:** Collection selection state
- **Button Ripple:** Click feedback animation

---

## Customization

### Colors
Edit the CSS variables in `:root`:
```css
:root {
  --accent-primary: #E36A3D; /* Change this */
  --bg-primary: #F5F1E8;
  /* etc. */
}
```

### Typography
Change font families in Google Fonts link:
```html
<!-- Line 10 in index.html -->
<link href="https://fonts.googleapis.com/css2?family=..." rel="stylesheet">
```

### Content
Edit the HTML content directly in `index.html`.

---

## Design Notes

- **No testimonials or fake stats** — Intentionally absent
- **No pricing tiers** — This is a concept project
- **No task/calendar features** — TUCK is specifically for saving items, not productivity management
- **Minimal cards** — Whitespace and typography do the heavy lifting
- **Asymmetric layouts** — Intentional visual rhythm, not generic symmetry

---

## Performance Tips

- Images are not included (add optimized images to `assets/images/`)
- All CSS is in two files for fast loading
- Vanilla JS means no framework overhead
- Lighthouse scores should be excellent

---

## Author

**Concept project by Aryan Bhujel**

© 2026 TUCK — A home for the things you save.

---

## License

This is a portfolio/concept project. Use freely for learning and portfolio purposes.
