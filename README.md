# jasperan Portfolio

A brutalist-style personal portfolio website for jasperan, AI Engineer and Developer Advocate.

## Versions

### 📄 **index.html** (Original)
- Clean, minimal brutalist design
- Fast loading with instant transitions
- Perfect for maximum accessibility
- Recommended for production use

### ✨ **index-enhanced.html** (Enhanced)
- Advanced animations and micro-interactions
- JetBrains Mono & Space Mono typography
- Custom cursor and visual effects
- Scroll-triggered animations
- Glitch effects and scanline overlay
- For those who want extra visual flair

**To use the enhanced version:** Rename `index-enhanced.html` to `index.html` or update your GitHub Pages settings.

## Design

This portfolio uses a **brutalist web design** aesthetic featuring:
- High contrast colors (black/white/red/yellow/cyan)
- Monospace typography
- Geometric shapes and sharp edges
- Visible grid borders
- Asymmetric layouts
- No rounded corners or subtle shadows

### Enhanced Version Additional Features:
- Animated grid background with noise texture
- Custom crosshair cursor
- Scanline effect overlay
- Scroll-triggered staggered animations
- Glitch text effects on hover
- Enhanced project card interactions with rotation
- Gradient timeline markers
- Floating geometric elements
- Pulsing border animations

## Tech Stack

- **HTML5** - Semantic structure
- **Tailwind CSS** - Utility-first styling via CDN
- **Vanilla JavaScript** - Minimal interactivity
- **No build process** - Just open `index.html` in a browser

## Features

- **Responsive design** - Works on mobile and desktop
- **Project showcase** - Filterable grid of open-source projects
- **Speaking timeline** - Visual timeline of conference appearances
- **Media integration** - Featured videos and articles
- **Smooth scrolling** - Between sections
- **Accessibility** - Keyboard navigation, focus states, semantic HTML

## Sections

1. **Hero** - Bold introduction with stats
2. **About** - Bio and current focus areas
3. **Projects** - Filterable project grid (AI/ML, Gaming, OSINT, Tools)
4. **Speaking** - Timeline of conference appearances (2022-2026)
5. **Media** - Featured videos and articles
6. **Contact** - Social links and contact information

## Local Development

Simply open `index.html` in your browser:

```bash
open index.html
# or
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Designed for GitHub Pages deployment:

1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source branch (main/master)
4. Site will be live at `https://username.github.io/repo-name`

## Customization

### Colors
Edit the Tailwind config in `index.html`:

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                'brutal-black': '#0A0A0A',
                'brutal-white': '#FAFAFA',
                'brutal-red': '#FF0000',
                'brutal-yellow': '#FFFF00',
                'brutal-cyan': '#00FFFF',
            }
        }
    }
}
```

### Content
Update the project cards, timeline items, and media sections directly in the HTML.

## Browser Support

Works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## Accessibility

- ✅ Keyboard navigation support
- ✅ Visible focus states
- ✅ Semantic HTML structure
- ✅ Alt text for images
- ✅ prefers-reduced-motion support
- ✅ 4.5:1 contrast ratio maintained

## Performance

- Single HTML file with CDN resources
- No build step required
- Minimal JavaScript
- Fast loading on all devices

## License

Open source. Feel free to use this template for your own portfolio.

## Credits

Built with:
- [Tailwind CSS](https://tailwindcss.com/)
- Brutalist design principles
- ❤️ and raw HTML

---

## 🎨 Frontend Design

### UI Screenshots

The portfolio features a **Brutalist Monospace** aesthetic with distinctive typography and bold visual elements.

#### Hero Section
![Hero](assets/screenshots/hero.png)
*Landing area with animated grid background and noise texture*

#### About Section
![About](assets/screenshots/about.png)
*Personal introduction with brutalist typography*

#### Projects Gallery
![Projects](assets/screenshots/projects.png)
*Showcase of AI and development projects*

#### Contact Section
![Contact](assets/screenshots/contact.png)
*Contact form with custom styling*

### Design System

| Component | Description |
|-----------|-------------|
| **Color Palette** | Soft violet (#8B5CF6), cyan (#06B6D4), slate dark backgrounds |
| **Typography** | JetBrains Mono + Space Mono monospace fonts |
| **Layout** | Asymmetric grids, bold borders, high contrast |
| **Effects** | Custom crosshair cursor, glitch animations, noise overlay |
| **Background** | Animated grid pattern with gradient mesh |

### Key UI Components

1. **Custom Cursor** - Crosshair SVG cursor replacing default pointer
2. **Glitch Text** - Animated text effects on hover
3. **Grid Background** - CSS-generated grid with subtle animation
4. **Noise Texture** - SVG noise overlay for tactile feel
5. **Project Cards** - Hover-reveal information with smooth transitions
6. **Social Links** - Icon buttons with color-coded hover states

> **Note**: Screenshots are stored in `assets/screenshots/`. Open index.html in a browser to capture updated screenshots.
