---
name: Radical Syntax
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1b1b1b'
  on-surface-variant: '#414a35'
  inverse-surface: '#303030'
  inverse-on-surface: '#f1f1f1'
  outline: '#717a62'
  outline-variant: '#c1caae'
  surface-tint: '#426900'
  primary: '#426900'
  on-primary: '#ffffff'
  primary-container: '#adff2f'
  on-primary-container: '#497300'
  inverse-primary: '#8fdb00'
  secondary: '#b40065'
  on-secondary: '#ffffff'
  secondary-container: '#e10080'
  on-secondary-container: '#fffbff'
  tertiary: '#626200'
  on-tertiary: '#ffffff'
  tertiary-container: '#f0f000'
  on-tertiary-container: '#6c6c00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#a8f928'
  primary-fixed-dim: '#8fdb00'
  on-primary-fixed: '#112000'
  on-primary-fixed-variant: '#314f00'
  secondary-fixed: '#ffd9e3'
  secondary-fixed-dim: '#ffb0ca'
  on-secondary-fixed: '#3e001f'
  on-secondary-fixed-variant: '#8d004e'
  tertiary-fixed: '#eaea00'
  tertiary-fixed-dim: '#cdcd00'
  on-tertiary-fixed: '#1d1d00'
  on-tertiary-fixed-variant: '#494900'
  background: '#f9f9f9'
  on-background: '#1b1b1b'
  surface-variant: '#e2e2e2'
typography:
  display-2xl:
    fontFamily: Syne
    fontSize: 96px
    fontWeight: '800'
    lineHeight: 90%
    letterSpacing: -0.04em
  display-lg:
    fontFamily: Syne
    fontSize: 64px
    fontWeight: '800'
    lineHeight: 100%
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Syne
    fontSize: 42px
    fontWeight: '800'
    lineHeight: 100%
  headline-md:
    fontFamily: Syne
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 110%
  body-lg:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 150%
  body-md:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 150%
  label-bold:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 120%
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 140%
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  border-weight-thick: 4px
  border-weight-thin: 2px
---

## Brand & Style

This design system embodies a **Neo-Brutalist** aesthetic tailored for the digital-native creator. It is high-energy, raw, and intentionally provocative, utilizing "ugly-cool" visual metaphors to break away from the sanitized minimalism of modern SaaS. The brand persona is bold and technical, celebrating the "under construction" energy of the web with a refined, contemporary edge.

The interface prioritizes raw structural elements: heavy strokes, unapologetic grids, and "sticker" components that feel slapped onto the canvas. It evokes an emotional response of confidence, transparency, and high-octane creativity.

## Colors

The palette is built on extreme contrast to ensure high visual impact. 
- **Primary (#ADFF2F):** A vibrant "GreenYellow" used for primary actions and background fills of key components.
- **Secondary (#FF1493):** A "DeepPink" used for highlights, secondary CTAs, and accent details.
- **Tertiary (#FFFF00):** A classic "Neon Yellow" for warning states or low-level accents.
- **Base:** The canvas remains #FFFFFF to allow the #000000 borders and neon fills to pop with maximum intensity.

Every interactive element must use a #000000 border to define its physical footprint.

## Typography

The typography system relies on a clash between the expressive, ultra-wide **Syne** for headlines and the rigid, technical **JetBrains Mono** for body content. 

Headlines should be set with tight leading and negative letter-spacing to create a "blocky" visual weight. All body copy and UI labels utilize monospace to lean into the developer/technical aesthetic. For mobile, display sizes scale aggressively downward to maintain readability while keeping the bold "impact" intact.

## Layout & Spacing

This design system uses a **Strict Grid Layout** where the grid itself is often made visible through background patterns or heavy borders.
- **The 4px Rule:** All primary borders are 4px. All spacing increments are multiples of 4px.
- **Intentional Overlap:** Components should frequently use "negative margins" to overlap one another, creating a layered, non-linear depth.
- **Grid:** A 12-column fluid grid on desktop with no rounded corners on the container. Margins are generous to allow the content to "breathe" within its heavy frames.
- **Marquee:** Large horizontal scrolls are used as separators between major sections, featuring auto-scrolling text in the secondary color.

## Elevation & Depth

Depth is conveyed through **Hard Shadows** rather than blurs. There are no soft ambient shadows in this system.
- **Level 1:** No shadow. Element sits flat on the background.
- **Level 2 (Active/Hover):** A 4px offset shadow (bottom-right) in #000000.
- **Level 3 (Floating/Sticker):** An 8px offset shadow in #000000.

The shadow color is always solid #000000 with 100% opacity. For a "pressed" effect, the element should translate 4px or 8px down and right to perfectly align with its shadow's original position.

## Shapes

The shape language is strictly **Sharp (0px)**. 90-degree angles reinforce the brutalist, architectural nature of the design. Rounding is only permitted for circular "sticker" accents or specific decorative icons. All interactive containers, input fields, and cards must maintain a 0px radius.

## Components

### Buttons
Buttons are chunky and high-contrast. 
- **Primary:** Primary color fill, 4px black border, 4px black hard shadow. Text is bold monospace.
- **Interaction:** On hover, the button shifts +2px; on click, it shifts +4px to "cover" the shadow.

### Cards (Sticker Style)
Cards use the Surface color (#F0F0F0) or Primary color fill. They must have a 4px black border. Content inside should have 24px padding. Use "floating" labels (labels that break the top border) for a technical feel.

### Input Fields
Inputs are white with 2px black borders. On focus, the border weight increases to 4px or changes to the Secondary color. Placeholder text should be 50% opacity black monospace.

### Chips/Tags
Small rectangular boxes with 2px borders. Use the Tertiary color (#FFFF00) for high-visibility tags like "NEW" or "LIVE."

### Marquee
A full-width container with a top and bottom 4px border. Text inside scrolls continuously. Used for branding, site-wide announcements, or social proof.