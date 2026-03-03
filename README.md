# jasperan Portfolio

A brutalist-style personal portfolio website for jasperan, AI Engineer and Developer Advocate.

## Design

This portfolio uses a **brutalist web design** aesthetic featuring:
- High contrast colors (black/white/red/yellow/cyan)
- Monospace typography
- Geometric shapes and sharp edges
- Visible grid borders
- Asymmetric layouts
- No rounded corners or subtle shadows

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
