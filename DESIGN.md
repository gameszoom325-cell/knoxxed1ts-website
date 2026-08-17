---
name: Technical Research Framework
colors:
  surface: '#141218'
  surface-dim: '#141218'
  surface-bright: '#3b383e'
  surface-container-lowest: '#0f0d13'
  surface-container-low: '#1d1b20'
  surface-container: '#211f24'
  surface-container-high: '#2b292f'
  surface-container-highest: '#36343a'
  on-surface: '#e6e0e9'
  on-surface-variant: '#cbc4d2'
  inverse-surface: '#e6e0e9'
  inverse-on-surface: '#322f35'
  outline: '#948e9c'
  outline-variant: '#494551'
  surface-tint: '#cfbcff'
  primary: '#cfbcff'
  on-primary: '#381e72'
  primary-container: '#6750a4'
  on-primary-container: '#e0d2ff'
  inverse-primary: '#6750a4'
  secondary: '#cdc0e9'
  on-secondary: '#342b4b'
  secondary-container: '#4d4465'
  on-secondary-container: '#bfb2da'
  tertiary: '#e7c365'
  on-tertiary: '#3e2e00'
  tertiary-container: '#c9a74d'
  on-tertiary-container: '#503d00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#cfbcff'
  on-primary-fixed: '#22005d'
  on-primary-fixed-variant: '#4f378a'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#cdc0e9'
  on-secondary-fixed: '#1f1635'
  on-secondary-fixed-variant: '#4b4263'
  tertiary-fixed: '#ffdf93'
  tertiary-fixed-dim: '#e7c365'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#141218'
  on-background: '#e6e0e9'
  surface-variant: '#36343a'
typography:
  display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  data-lg:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '500'
    lineHeight: '1.4'
  data-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
  data-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  grid_columns: '12'
  gutter: 16px
  margin: 24px
---

## Brand & Style

The design system is engineered for high-density information environments, research data visualization, and academic publishing. The aesthetic is rooted in **Modern Minimalism with a Technical/Lab influence**, prioritizing clarity, precision, and structural integrity.

The personality is authoritative yet transparent. It avoids decorative elements in favor of functional indicators, drawing inspiration from blueprint schematics, engineering consoles, and peer-reviewed journals. Visual hierarchy is established through a rigorous grid and thin, precise borders rather than depth or shadows.

## Colors

This design system utilizes two distinct themes optimized for different research environments: a high-focus **Dark Mode** for laboratory monitors and data terminals, and a **Light Mode** optimized for long-form reading and printed documentation.

- **Primary:** Used for actionable elements, progress indicators, and active states.
- **Secondary:** Reserved for "Success" states, validated data points, and environmental parameters.
- **Accent:** Applied to variables, probability warnings, and highlighted mathematical constants.
- **Neutral/Border:** A strict 1px border system replaces shadows to define containment and separation.

## Typography

The typography strategy is bifurcated between **Inter** for prose and interface navigation, and **JetBrains Mono** for all technical outputs.

- **Sans-Serif (Inter):** Leverages the tall x-height for maximum legibility in complex dashboards. Used for headers, body copy, and navigation.
- **Monospace (JetBrains Mono):** Used for mathematical equations, variable names, data tables, and coordinate systems. It ensures character alignment in vertical data stacks.
- **Mobile Scaling:** Large displays scale down by 20% on mobile devices, while data-sm remains constant to preserve readability of technical specifications.

## Layout & Spacing

The system employs a **Modular Fixed Grid** based on 4px increments. Layouts should feel "packed" but organized, reflecting the density of scientific documentation.

- **Grid:** A 12-column layout on desktop, transitioning to 6-column on tablet and 2-column on mobile.
- **Rhythm:** Use `md` (16px) for standard component padding and `sm` (8px) for internal element grouping (e.g., label to input).
- **Alignment:** Content should always be hard-aligned to the grid lines. Components should utilize the full width of their allocated columns to maintain a "tabular" appearance.

## Elevation & Depth

This design system rejects depth-based hierarchy (shadows). Instead, it uses **Structural Tiering**:

- **Borders:** All containers, cards, and sections are defined by 1px solid borders.
- **Surface Contrast:** Background shifts (e.g., moving from `#0f172a` to `#1e293b`) denote hierarchy.
- **Active States:** Instead of a shadow, an active element is indicated by a primary-colored border or a high-contrast fill.
- **Backdrop:** Overlays use a slight dimming effect (30% opacity) without blur to maintain technical clarity of underlying data.

## Shapes

The shape language is rigid and precise. 
- **Standard Radius:** 4px (`rounded-sm`) for buttons, inputs, and cards.
- **Interactive Elements:** Checkboxes and radio buttons remain sharp or use minimal rounding to differentiate from organic/consumer UI.
- **Icons:** Use stroke-based icons with a 1.5px or 2px weight to match the border-driven aesthetic.

## Components

- **Buttons:** Rectangular with 4px radius. Primary buttons use a solid fill; secondary buttons use a 1px border. Focus states must feature a 2px offset ring.
- **Input Fields:** Bottom-aligned labels using `data-sm` typography. The input box uses a subtle background fill and a 1px bottom border that expands to a full box on focus.
- **Data Tables:** No vertical borders. Use thin horizontal dividers. Header cells use `data-sm` in all-caps with a subtle background tint.
- **Status Chips:** Small, rectangular indicators. Use `secondary` for "nominal" and `accent` for "deviation."
- **Cards:** No shadows. Defined by 1px borders. Use a "header bar" within the card (a slightly different surface color) to categorize data.
- **Code/Math Blocks:** Enclosed in a surface-colored container with `data-md` text and syntax highlighting that mirrors the system's primary/secondary/accent palette.