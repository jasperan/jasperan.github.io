# jasperan Portfolio - Brutalist Design System

**Project:** Personal Portfolio Website  
**Style:** Brutalist/Experimental  
**Target:** Full-featured portfolio with projects, speaking, media, and contact

## Design Philosophy

Brutalist web design embraces raw, unconventional aesthetics with:
- High contrast color schemes (black/white/bold accents)
- Bold, unconventional typography
- Geometric shapes and sharp edges
- Minimal decoration, maximum impact
- Intentionally "undesigned" appearance
- Grid-based layouts with visible structure

## Color Palette

### Primary Colors
- **Background:** `#0A0A0A` (near black)
- **Text Primary:** `#FAFAFA` (off-white)
- **Text Secondary:** `#A0A0A0` (gray)
- **Accent 1:** `#FF0000` (pure red - brutalist red)
- **Accent 2:** `#FFFF00` (pure yellow)
- **Accent 3:** `#00FFFF` (cyan)

### Functional Colors
- **Borders:** `#FFFFFF` (white borders, thick)
- **Hover States:** `#FF0000` background with white text
- **Links:** `#FFFF00` with underline
- **Code/Tech:** `#00FFFF`

## Typography

### Font Stack
- **Headings:** `monospace` (Courier New, Consolas, monospace)
- **Body:** `system-ui, -apple-system, sans-serif`
- **Accent Text:** `monospace` with letter-spacing

### Scale
- **Hero Title:** `clamp(3rem, 10vw, 8rem)` - massive, impactful
- **Section Headers:** `clamp(2rem, 5vw, 4rem)`
- **Body:** `clamp(1rem, 2vw, 1.25rem)`
- **Small:** `0.875rem`

## Layout Principles

### Grid System
- Use visible grid borders (3px solid white)
- Asymmetric layouts encouraged
- Overlapping elements for depth
- Large whitespace between sections

### Spacing
- **Section padding:** `4rem 2rem`
- **Element spacing:** `2rem` minimum
- **Border thickness:** `3px` for visual impact

### Components

#### Hero Section
- Full viewport height
- Massive typography
- Geometric shapes (rectangles, lines)
- Asymmetric layout
- Bold accent color blocks

#### Project Grid
- Visible grid borders
- Mix of large and small cards
- Category filters with brutalist buttons
- Hover effects: background color fill
- Tech stack tags in monospace

#### Timeline (Speaking/Events)
- Vertical line with geometric markers
- Alternating left/right layout
- Bold dates in accent color
- Event names in large monospace

#### Media Section
- Embedded content in bordered frames
- Video thumbnails with bold overlays
- Article cards with accent borders

#### Contact Section
- Large, prominent links
- Geometric social icons
- Email in monospace

## Visual Effects

### Animations
- **Hover:** Instant color transitions (no easing)
- **Scroll:** Snap scrolling between sections
- **Load:** Staggered appearance (100ms delay per element)

### Borders & Lines
- Thick borders (3-4px)
- No border-radius (sharp corners)
- Geometric shapes only
- Visible grid lines

## Accessibility

Despite brutalist aesthetic:
- Maintain 4.5:1 contrast ratio
- Visible focus states (thick outline)
- Keyboard navigation support
- Semantic HTML structure
- Alt text for images
- prefers-reduced-motion support

## Anti-Patterns to Avoid

❌ Rounded corners  
❌ Subtle shadows  
❌ Smooth transitions  
❌ Pastel colors  
❌ Thin borders  
❌ Traditional navigation bars  
❌ Centered layouts (use asymmetric)  
❌ Decorative illustrations

## Technology Stack

- **HTML5** - Semantic structure
- **Tailwind CSS** - Utility-first styling
- **Vanilla JavaScript** - Minimal interactivity
- **No frameworks** - Keep it raw and fast

## Content Structure

1. **Hero** - Name, title, brief intro with geometric shapes
2. **About** - Quick bio with accent blocks
3. **Projects** - Filterable grid with categories
4. **Speaking** - Timeline of events and appearances
5. **Media** - Videos and articles in bordered frames
6. **Contact** - Large links to GitHub, LinkedIn, email

## Deployment

- **Platform:** GitHub Pages
- **Build:** Static HTML, no build process needed
- **Domain:** Can use custom domain or GitHub Pages default
