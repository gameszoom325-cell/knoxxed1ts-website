---
name: KNOXXED1TS
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#ccc3da'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#958da3'
  outline-variant: '#4a4457'
  surface-tint: '#d1bcff'
  primary: '#d1bcff'
  on-primary: '#3c0090'
  primary-container: '#7000ff'
  on-primary-container: '#ddcdff'
  inverse-primary: '#7212ff'
  secondary: '#a6e6ff'
  on-secondary: '#003543'
  secondary-container: '#14d1ff'
  on-secondary-container: '#00566b'
  tertiary: '#ffb1c3'
  on-tertiary: '#66002c'
  tertiary-container: '#b60055'
  on-tertiary-container: '#ffc5d1'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d1bcff'
  on-primary-fixed: '#23005b'
  on-primary-fixed-variant: '#5700c9'
  secondary-fixed: '#b7eaff'
  secondary-fixed-dim: '#4cd6ff'
  on-secondary-fixed: '#001f28'
  on-secondary-fixed-variant: '#004e60'
  tertiary-fixed: '#ffd9e0'
  tertiary-fixed-dim: '#ffb1c3'
  on-tertiary-fixed: '#3f0019'
  on-tertiary-fixed-variant: '#8f0041'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1440px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

The design system is built for a high-performance anime editing community, where the interface acts as a cinematic frame for high-motion content. The brand personality is aggressive, futuristic, and premium—drawing heavy influence from high-end gaming hardware interfaces and modern cyberpunk aesthetics.

The visual style is **Cinematic Glassmorphism**. It utilizes deep, ink-like blacks as a foundation, layered with translucent frosted-glass surfaces that "catch" the light from vibrant accent colors. The interface feels like a heads-up display (HUD), emphasizing depth through blurred background glows, microscopic borders, and subtle neon light-leaks.

**Key Visual Principles:**
- **Atmospheric Depth:** Use semi-transparent layers to allow background "particle" or "glow" assets to bleed through the UI.
- **Precision:** Thin, high-contrast strokes define element boundaries, replacing heavy shadows.
- **Motion-Ready:** The UI remains static and minimal to ensure that video thumbnails and motion graphics remain the focal point.

## Colors

This design system utilizes a "Void" palette, where the primary canvas is near-black to maximize the luminosity of the accent colors. 

- **Primary (Electric Violet):** Used for high-action triggers, active states, and primary brand accents.
- **Secondary (Cyber Blue):** Used for data visualization, secondary actions, and "cooling" the palette.
- **Tertiary (Neon Pink):** Reserved exclusively for "Heat" or "Trending" indicators and critical notifications.
- **Surface Tiers:**
  - `Surface-Base`: #050505 (Solid)
  - `Surface-Glass`: rgba(255, 255, 255, 0.03) with 20px backdrop blur.
  - `Surface-Overlay`: rgba(255, 255, 255, 0.08) for elevated hover states.

## Typography

The typography strategy balances high-impact display moments with technical precision.

- **Headlines:** Use **Space Grotesk** for all titles. Its geometric, technical quirks echo the digital nature of video editing. Tighten letter-spacing on larger sizes for a more "locked-in" look.
- **Body:** **Inter** provides a neutral, highly readable foundation for community comments and video descriptions.
- **Technical/Metadata:** **JetBrains Mono** is used for timestamps, file sizes, and technical specifications (FPS, resolution) to evoke a "code" or "editor" feel.

## Layout & Spacing

The layout follows a strict 12-column grid for desktop with generous outer margins to focus the eye toward the center of the screen.

- **Content Reflow:** On desktop, the "Video Grid" uses a fluid 3 or 4 column span. On mobile, this collapses into a single-column stack with full-bleed edges to maximize video visibility.
- **Rhythm:** Use multiples of 4px. Grids should feel "airy" with 24px gutters to allow the glassmorphic background blurs to be visible between components.
- **Safe Zones:** High-intensity backgrounds (particles/grids) should be constrained to a lower z-index "Environment Layer," while the content sits in a "Glass Container" with at least 40px of internal padding.

## Elevation & Depth

This system ignores traditional shadows in favor of **Luminous Elevation**.

1.  **Level 0 (The Void):** Background color #050505.
2.  **Level 1 (The Glass):** A 1px stroke (rgba(255,255,255,0.1)) + backdrop-filter: blur(20px). No background color or very low opacity white (3%).
3.  **Level 2 (The Glow):** Elements that are interactive or "Live" emit a 15px-30px diffused outer glow using the Primary or Secondary color at 20% opacity.
4.  **Z-Indexing:**
    *   `Environment`: -1 (Gradients/Particles)
    *   `Content`: 1 (Cards/Text)
    *   `Navigation`: 10 (Fixed Glass Bar)
    *   `Modals`: 100 (Full-screen overlay with 40px blur)

## Shapes

The shape language is "Modern Geometric." 

- **Primary Radius:** 0.5rem (8px) for cards and buttons. This provides a clean, modern feel without looking too playful or too industrial.
- **Large Radius:** 1.5rem (24px) for hero containers or featured video highlights.
- **Micro-details:** Use 45-degree chamfered corners on very small labels (like "4K" or "HD" badges) to enhance the tech/gaming aesthetic.

## Components

**Buttons:**
- **Primary:** Solid #7000FF background with a subtle white inner-top border (0.5px) for a "lit from above" effect. Hover state triggers a #7000FF outer glow.
- **Ghost:** Transparent background with 1px #00D1FF border. Text in #00D1FF.

**Video Cards:**
- High-contrast thumbnails with 8px rounded corners.
- On hover: The 1px border transitions from transparent to the Primary color, and the background glass opacity increases slightly.
- Metadata (User, Views) uses the `label-caps` typography style.

**Navigation Bar:**
- A floating glass "pill" or full-width bar.
- `backdrop-filter: blur(30px)`.
- Bottom border only: 1px rgba(255,255,255,0.05).

**Input Fields:**
- Dark background (#111), 8px radius, 1px border (rgba(255,255,255,0.1)).
- Focus state: Border changes to Electric Blue (#00D1FF) with a 2px blue outer glow.

**Chips/Badges:**
- Small, uppercase text.
- Use Secondary or Tertiary colors with 10% background opacity for categorized content (e.g., "AMV", "Edit", "Tutorial").