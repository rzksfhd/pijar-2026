# PIJAR 2026 Design System

## Brand Identity

### Name
**PIJAR** - Program for Innovation and Joint Action for Resilience
**Tagline**: Pertukaran Ilmu dan Pelajar

### Theme
"Beyond Distance: Connecting Global Minds for Sustainable Development"

---

## Brand Colors

### Primary Palette

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Primary Green | `#059669` | 5, 150, 105 | Primary CTAs, headings |
| Primary Dark | `#047857` | 4, 120, 87 | Hover states, accents |
| Primary Light | `#10B981` | 16, 185, 129 | Highlights, gradients |

### Secondary Palette

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Sky Blue | `#0EA5E9` | 14, 165, 233 | Secondary elements, gradients |
| Amber | `#F59E0B` | 245, 158, 11 | Accent, warnings, badges |

### Neutral Palette

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Dark | `#1E293B` | 30, 41, 59 | Text, headings |
| Gray | `#64748B` | 100, 116, 139 | Body text, secondary |
| Light | `#F1F5F9` | 241, 245, 249 | Backgrounds, sections |
| White | `#FFFFFF` | 255, 255, 255 | Cards, containers |

### Gradient Combinations

```css
/* Hero gradient */
background: linear-gradient(135deg, #ECFDF5 0%, #E0F2FE 50%, #FEF3C7 100%);

/* Primary gradient (buttons) */
background: linear-gradient(135deg, #059669, #047857);

/* Icon gradient */
background: linear-gradient(135deg, #10B981, #0EA5E9);
```

---

## Typography

### Font Family
**Plus Jakarta Sans** (Google Fonts)
- Modern, clean, highly legible
- Alternative: Inter

### Type Scale

| Element | Size | Weight | Line Height | Usage |
|---------|------|--------|-------------|-------|
| H1 | 3.5rem (56px) | 800 | 1.1 | Hero title |
| H2 | 2.5rem (40px) | 800 | 1.2 | Section titles |
| H3 | 1.25rem (20px) | 700 | 1.4 | Card titles |
| H4 | 1.125rem (18px) | 600 | 1.5 | Subheadings |
| Body | 1rem (16px) | 400 | 1.7 | Paragraph text |
| Body Large | 1.125rem (18px) | 500 | 1.6 | Lead paragraphs |
| Small | 0.875rem (14px) | 400 | 1.5 | Captions, labels |
| Button | 1rem (16px) | 600 | 1 | Button text |

---

## Components

### Buttons

**Primary Button**
```css
.btn-primary {
    background: linear-gradient(135deg, #059669, #047857);
    color: #FFFFFF;
    padding: 0.875rem 1.75rem;
    border-radius: 50px;
    font-weight: 600;
    box-shadow: 0 4px 15px rgba(5, 150, 105, 0.3);
    transition: all 0.3s;
}
.btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(5, 150, 105, 0.4);
}
```

**Secondary Button**
```css
.btn-secondary {
    background: transparent;
    color: #059669;
    border: 2px solid #059669;
    border-radius: 50px;
}
.btn-secondary:hover {
    background: #059669;
    color: #FFFFFF;
}
```

**White Button**
```css
.btn-white {
    background: #FFFFFF;
    color: #059669;
    border-radius: 50px;
}
```

### Cards

**Highlight Card**
```css
.highlight-card {
    background: #FFFFFF;
    padding: 2rem;
    border-radius: 1rem;
    border: 1px solid rgba(0,0,0,0.05);
    transition: all 0.3s;
}
.highlight-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 40px rgba(0,0,0,0.1);
}
```

**Funding Card (Dark)**
```css
.funding-card {
    background: linear-gradient(135deg, #059669, #047857);
    color: #FFFFFF;
    padding: 2.5rem;
    border-radius: 1.5rem;
    box-shadow: 0 20px 50px rgba(5, 150, 105, 0.3);
}
```

### Icons

**Icon Container**
```css
.highlight-icon {
    width: 70px;
    height: 70px;
    background: linear-gradient(135deg, #10B981, #0EA5E9);
    border-radius: 1rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
}
```

**Number Badge**
```css
.format-number {
    position: absolute;
    top: -15px;
    width: 30px;
    height: 30px;
    background: #059669;
    color: #FFFFFF;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
}
```

### Badges & Tags

**Section Tag**
```css
.section-tag {
    background: linear-gradient(135deg, rgba(5, 150, 105, 0.1), rgba(14, 165, 233, 0.1));
    color: #059669;
    padding: 0.5rem 1rem;
    border-radius: 50px;
    font-size: 0.875rem;
    font-weight: 600;
}
```

**Hero Badge**
```css
.hero-badge {
    background: #FFFFFF;
    color: #059669;
    padding: 0.5rem 1rem;
    border-radius: 50px;
    font-weight: 600;
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}
```

**Hours Badge**
```css
.hours-badge {
    background: #F59E0B;
    color: #1E293B;
    padding: 0.75rem 1.5rem;
    border-radius: 50px;
    font-weight: 700;
}
```

---

## Layout

### Container
- Desktop: `max-width: 1200px`
- Padding: `0 1.5rem`
- Centered: `margin: 0 auto`

### Section Spacing
- Padding vertical: `5rem` (80px)
- Header margin bottom: `3rem` (48px)

### Grid System

**Highlights Grid**
```css
grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
gap: 1.5rem;
```

**Two Column**
```css
grid-template-columns: 1fr 1fr;
gap: 4rem;
```

**Four Column**
```css
grid-template-columns: repeat(4, 1fr);
gap: 1.5rem;
```

---

## Responsive Breakpoints

| Breakpoint | Width | Target |
|------------|-------|--------|
| Desktop | > 1024px | Laptops, desktops |
| Tablet | 769px - 1024px | Tablets, small laptops |
| Mobile | < 768px | Smartphones |

### Mobile Adjustments
- Hero title: `2.25rem`
- Section title: `2rem`
- Hide navigation links
- Single column grids
- Stack buttons vertically

---

## Animation Guidelines

### Hover Effects
```css
transition: all 0.3s ease;
```

### Transforms
- Card lift: `translateY(-5px)`
- Button lift: `translateY(-2px)`

### Float Animation (Hero Badge)
```css
@keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
}
```

---

## Page Structure

### Navigation
- Fixed position
- White background with blur
- Shadow: `0 1px 3px rgba(0,0,0,0.1)`
- Z-index: 1000

### Hero Section
- Padding: `10rem top, 6rem bottom`
- Background: Light gradient (green/blue/yellow tints)
- Content: Centered, max-width 800px
- Stats row below main content

### Sections Order
1. Hero (gradient background)
2. Program Highlights (light gray)
3. Benefits (white)
4. Program Format (light gray)
5. Timeline (green gradient)
6. Eligibility (white)
7. CTA (dark)
8. Footer (darker)

---

## Emoji Usage

### Navigation
- Logo: 🌍 (global/earth)

### Highlights
- 📖 Lectures & Workshops
- 🌏 Field Visits
- 🤝 Collaboration
- 🏛 Cultural Heritage
- 💡 Group Projects
- 🎯 Final Presentation

### Benefits
- 🎓 Certificate
- 🌐 Network
- 📚 Learning
- 🤝 Collaboration
- 💰 Funding

### Timeline
- 🗓️ Calendar
- 📍 Location
- 🇮🇩 Indonesia

### CTA
- 🔥 Ignite/Action
- 👉 Apply pointer
- 📖 Learn More

---

## File Structure

```
pijar-2026/
├── index.html          # Landing page
├── ROADMAP.md          # Program roadmap
├── DESIGN_SYSTEM.md    # This document
├── README.md           # Project readme
├── css/
│   └── styles.css      # Compiled styles
├── images/
│   ├── logo.svg        # PIJAR logo
│   ├── hero-bg.jpg     # Hero background
│   └── gallery/        # Program photos
└── assets/
    └── favicon.ico     # Site favicon
```

---

## Design Principles

1. **International Appeal**: Clean, professional, welcoming to global audience
2. **SDG Focus**: Green/blue palette reflects sustainability theme
3. **Mobile-First**: Responsive design for all devices
4. **Clear CTAs**: Prominent registration buttons throughout
5. **Cultural Pride**: Indonesian identity without being overwhelming
6. **Trust Building**: University branding, clear information hierarchy

---

*Version: 1.0*
*Last Updated: April 2026*