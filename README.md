# Modern Portfolio

A clean, accessible portfolio with warm aesthetics and full WCAG AA compliance.

## Design Philosophy

This portfolio focuses on clarity and readability:
- **Warm Neutrals**: Cream (#FAF8F5) and charcoal (#1A1816) backgrounds
- **Bold Accent Colors**: Orange, mustard, and teal palette
- **Clean Typography**: System fonts with clear hierarchy
- **Generous Whitespace**: Breathing room for content
- **Dynamic Layout**: Staggered stats cards with colored accent bars
- **Subtle Interactions**: Refined hover states and transitions

## Key Features

### Accessibility (WCAG AA Compliant)
- ✅ All text meets 4.5:1 contrast ratio
- ✅ Large text meets 3:1 contrast ratio
- ✅ Keyboard navigation support
- ✅ Screen reader friendly
- ✅ Focus indicators visible
- ✅ Respects reduced motion preferences
- ✅ Semantic HTML5 structure

### Color Palette
- **Orange** (#D0722E): Primary accent for links and interactions
- **Mustard** (#B8851E): Secondary accent for variety
- **Teal** (#3B8B8B): Tertiary accent for balance
- All colors tested and adjusted for accessibility

### Responsive Design
- Mobile-first approach
- Fluid typography with `clamp()`
- CSS Grid for flexible layouts
- Breakpoints: 768px (tablet), 1024px (desktop)

### Dark Mode Support
- Automatic switching based on system preferences
- Warm charcoal background for comfortable viewing
- All colors re-optimized for dark mode contrast

### Modern CSS Features
- CSS Custom Properties (variables) for easy theming
- Modern layout with Grid and Flexbox
- Hardware-accelerated animations
- Print-optimized styles
- Staggered card layout with dynamic positioning

## File Structure

```
modernized/
├── index.html              # Semantic HTML5 structure
├── styles.css              # Modern CSS with variables
├── favicon.svg             # Tri-color gradient ampersand
├── apple-touch-icon.png    # 180×180 icon for iOS
└── README.md               # This file
```

## Color System

### Light Mode
```css
--color-bg: #FAF8F5;           /* Warm cream background */
--color-text: #0a0a0a;         /* Near-black text */
--color-text-secondary: #6A6A6A;  /* Medium gray */
--color-accent: #D0722E;       /* Primary orange */
--color-orange: #D0722E;       /* Orange accent */
--color-mustard: #B8851E;      /* Mustard accent */
--color-teal: #3B8B8B;         /* Teal accent */
```

### Dark Mode
```css
--color-bg: #1A1816;           /* Warm charcoal */
--color-text: #f5f5f5;         /* Off-white */
--color-accent: #E89060;       /* Lighter orange for dark */
```

## Customization

All design tokens are CSS variables at the top of `styles.css`. Modify them to customize:

**Change accent colors:**
```css
:root {
  --color-orange: #your-color;
  --color-mustard: #your-color;
  --color-teal: #your-color;
}
```

**Adjust spacing:**
```css
:root {
  --space-xl: 2rem;   /* Increase/decrease overall spacing */
}
```

**Modify backgrounds:**
```css
:root {
  --color-bg: #ffffff;  /* Switch back to pure white */
}
```

## Performance

- **No external dependencies**: System fonts only
- **Preloaded CSS**: Faster initial render
- **Optimized icons**: SVG + PNG for broad support
- **Minimal DOM**: Clean, semantic structure
- **Hardware acceleration**: Smooth animations

## Browser Support

Works in all modern browsers:
- Chrome/Edge 88+
- Firefox 78+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

Note: Uses modern CSS features like `color-mix()` and `clamp()`.

## Accessibility Testing

All color combinations tested with WCAG contrast calculator:
- Main text: 17+:1 ratio ✅
- Secondary/tertiary text: 4.5+:1 ratio ✅
- Large stat numbers: 3+:1 ratio ✅
- Interactive elements: Proper focus states ✅

## Development Notes

### Icons
- `favicon.svg`: Tri-color gradient ampersand with warm backgrounds
- `apple-touch-icon.png`: Generated from SVG at 180×180px
- Both adapt to light/dark mode

### Typography Scale
```
h1: clamp(2.25rem, 5vw + 1rem, 4rem)
h2: clamp(1.5rem, 3vw + 0.5rem, 2rem)
h3: clamp(1.125rem, 1.5vw + 0.5rem, 1.125rem)
```

### Spacing Scale
```
--space-xs:  0.5rem   (8px)
--space-sm:  0.75rem  (12px)
--space-md:  1rem     (16px)
--space-lg:  1.5rem   (24px)
--space-xl:  2rem     (32px)
--space-2xl: 2.5rem   (40px)
--space-3xl: 3rem     (48px)
--space-4xl: 4rem     (64px)
```

## License

© 2026 Justin Sepulveda
