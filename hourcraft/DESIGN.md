---
name: Hourcraft
colors:
  surface: '#131314'
  surface-dim: '#131314'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1c1c'
  surface-container: '#1f2020'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#343535'
  on-surface: '#e4e2e2'
  on-surface-variant: '#bdcbae'
  inverse-surface: '#e4e2e2'
  inverse-on-surface: '#303030'
  outline: '#88957b'
  outline-variant: '#3e4a34'
  surface-tint: '#6ee000'
  primary: '#f7ffe9'
  on-primary: '#173800'
  primary-container: '#7cfc00'
  on-primary-container: '#347000'
  inverse-primary: '#316b00'
  secondary: '#a1d494'
  on-secondary: '#0a3909'
  secondary-container: '#23501e'
  on-secondary-container: '#90c283'
  tertiary: '#fffbff'
  on-tertiary: '#3f2d1e'
  tertiary-container: '#f8dac4'
  on-tertiary-container: '#755e4d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#82ff1a'
  primary-fixed-dim: '#6ee000'
  on-primary-fixed: '#0a2000'
  on-primary-fixed-variant: '#245100'
  secondary-fixed: '#bcf0ae'
  secondary-fixed-dim: '#a1d494'
  on-secondary-fixed: '#002201'
  on-secondary-fixed-variant: '#23501e'
  tertiary-fixed: '#fbddc7'
  tertiary-fixed-dim: '#dec1ac'
  on-tertiary-fixed: '#28180b'
  on-tertiary-fixed-variant: '#574333'
  background: '#131314'
  on-background: '#e4e2e2'
  surface-variant: '#343535'
typography:
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-sm:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '700'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
spacing:
  base: 4px
  unit-1: 4px
  unit-2: 8px
  unit-4: 16px
  unit-8: 32px
  gutter: 16px
  margin: 24px
---

## Brand & Style
The design system for this internal management application balances the rigorous organization of an enterprise tool with the distinct, voxel-based aesthetic of the Minecraft universe. The brand personality is industrious, methodical, and structural.

The design style is **Modern Voxel-Brutalism**. It utilizes sharp geometric forms, high-contrast borders, and subtle 3D "extrusion" effects to mimic the feeling of stacked blocks. While the interface is playful, it maintains a "Corporate Professional" standard through disciplined alignment, clear information hierarchy, and a restrained use of ornamentation. Whitespace is used not for airiness, but to define "building blocks" of data.

## Colors
This design system defaults to a **Dark Mode** environment to emphasize the richness of the forest and stone palette.

- **Primary (#7CFC00):** A high-vibrancy "Lime Grass" used exclusively for active states, primary calls to action, and positive indicators.
- **Secondary (#2D5A27):** "Deep Forest" green used for sidebar backgrounds and secondary navigational elements.
- **Tertiary (#4A3728):** "Earth Brown" used for header accents and specific organizational categories like "Shifts" or "Logs."
- **Neutral (#4E4E4E):** "Stone Gray" serves as the primary surface color for cards and containers.
- **Warning (#FFA500):** Used for maintenance alerts and critical system messages.

Backgrounds should use a near-black #121212 to allow the "block" containers to pop, while text should remain high-contrast (Off-white #F5F5F5) for legibility.

## Typography
The system employs a dual-font strategy. **Space Grotesk** is used for headlines and UI accents; its geometric, almost monospaced construction provides the "blocky" feel of Minecraft while remaining professional and modern. **Inter** is used for all body copy, data tables, and dense information sets to ensure maximum readability and a "SaaS" feel.

- **Headlines:** Always Bold. Use uppercase for smaller sub-headers to evoke the "Inventory" screen feel.
- **Body:** Standard weight. Use for all user-generated content and data.
- **Labels:** Use for badges, table headers, and button text to maintain the "voxel" character throughout the UI.

## Layout & Spacing
The layout is governed by a strict **8px grid system**. Everything must align to this grid to reinforce the "built from blocks" metaphor. 

- **Grid:** Use a 12-column fluid grid for desktop with 16px gutters. 
- **Containers:** Content should be housed in "Voxel Cards" that utilize 16px or 24px internal padding.
- **Stacking:** Elements should never feel floating. Use tight spacing (4px or 8px) between related items to create a sense of solid construction.
- **Responsive:** On mobile, margins reduce to 16px and the 12-column grid collapses to a single column, but the "block" styling of components remains rigid.

## Elevation & Depth
Elevation in this design system is achieved through **Voxel Extrusion** rather than traditional soft shadows.

- **The Voxel Effect:** Instead of `box-shadow`, use a 2px to 4px solid bottom border of a darker shade to create a "thick block" look. 
- **Layers:** 
    - **Level 0 (Floor):** Background color.
    - **Level 1 (Ground):** Main UI containers (Stone Gray) with a 4px dark bottom border.
    - **Level 2 (Object):** Buttons and interactives, which "depress" (remove the bottom border and translate Y +2px) when clicked.
- **Borders:** Use high-contrast 2px solid borders for all containers. Avoid blurs. Every edge should be sharp and defined.

## Shapes
In keeping with the Minecraft aesthetic, the shape language is **strictly orthogonal**. 

- **Corners:** 0px (Sharp) is the default for all buttons, inputs, and containers. 
- **Accents:** Only use a 4px "step" (inner notch) if a distinction is needed for specific UI items like role badges.
- **Icons:** Use thick-stroke (2px) linear icons or pixel-art style icons. Avoid rounded or organic icon sets.

## Components

### Buttons
Buttons are styled as "Blocks." 
- **Default:** Solid color with a 4px darker bottom border.
- **Hover:** Brighten the background color slightly.
- **Active (Pressed):** Remove the bottom border and move the button down 4px to simulate a physical press into the grid.

### Data Tables
Tables should look like a "Blueprint." Use `Stone Gray` for header rows with `Label-Caps` typography. Cell borders should be 1px solid `#333333`. Row hovering should highlight the entire row in a translucent `Primary` green tint.

### Shift Cards & Role Badges
- **Shift Cards:** Use `Stone Gray` blocks with a vertical color-strip on the left to indicate the shift status (Active = Green, Maintenance = Orange).
- **Role Badges:** Small, sharp-edged rectangles using the `Earth Brown` or `Deep Forest` palette with white text.

### Inputs
Fields should have a 2px solid border. The "focus" state is indicated by a 2px `Primary` green outline. No inner shadows; keep the field flat and solid.

### Status Indicators
Use literal "Status Blocks"—small 12x12px solid squares. 
- **Active:** #7CFC00
- **Archived:** #4E4E4E
- **Maintenance:** #FFA500

### Alert Banners
Banners span the full width of their container. They do not have rounded corners. They use a high-contrast background (e.g., Warning Orange) with black text for maximum urgency.