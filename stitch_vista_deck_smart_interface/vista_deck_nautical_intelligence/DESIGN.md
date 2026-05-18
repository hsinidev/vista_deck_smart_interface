---
name: Vista-Deck Nautical Intelligence
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#bec7d4'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#88919d'
  outline-variant: '#3f4852'
  surface-tint: '#98cbff'
  primary: '#98cbff'
  on-primary: '#003354'
  primary-container: '#00a3ff'
  on-primary-container: '#00375a'
  inverse-primary: '#00629d'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#a8c9f3'
  on-tertiary: '#0a3254'
  tertiary-container: '#7f9fc7'
  on-tertiary-container: '#103658'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#cfe5ff'
  primary-fixed-dim: '#98cbff'
  on-primary-fixed: '#001d33'
  on-primary-fixed-variant: '#004a77'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#d1e4ff'
  tertiary-fixed-dim: '#a8c9f3'
  on-tertiary-fixed: '#001d36'
  on-tertiary-fixed-variant: '#27496c'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: metropolis
    fontSize: 48px
    fontWeight: '300'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: metropolis
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-md:
    fontFamily: metropolis
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: metropolis
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: metropolis
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.08em
  headline-lg-mobile:
    fontFamily: metropolis
    fontSize: 28px
    fontWeight: '400'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-padding: 40px
  gutter: 24px
  card-gap: 32px
  safe-area: env(safe-area-inset-bottom)
---

## Brand & Style
The design system embodies the intersection of maritime luxury and advanced environmental engineering. The brand personality is "Technological Serenity"—a balance of high-performance glass-control systems and the tranquil, expansive nature of the ocean. It targets high-net-worth yacht owners and captains who value clarity, precision, and immersive aesthetics.

The visual style is a refined **Fluid-Modern Glassmorphism**. It utilizes multi-layered translucent surfaces that mimic the property of smart glass. The emotional response should be one of "Unobstructed Vision," where the interface feels like an extension of the yacht’s windows rather than a digital overlay. Lighting is central to the experience, using soft, ethereal glows that suggest light passing through deep water and polished crystalline structures.

## Colors
This design system utilizes a "Deep Sea" palette to maintain night-vision compatibility and luxury appeal. The primary **Azure Blue** serves as the functional highlight for active states and critical environmental data. **White** is used sparingly for high-readability text and "Polished Glass" specular highlights.

The background is not a solid black, but a deep, spectral Navy (`#0F172A`) that provides the necessary contrast for glass effects. Functional accents utilize gradients transitioning from Azure to a deeper Cyan to simulate the movement of water and light through thick glass panels.

## Typography
The typographic choice focuses on geometric precision and clarity. **Metropolis** provides the structural, modern sans-serif feel required for architectural interfaces. Headlines should use lighter weights (`300` or `400`) to maintain an airy, sophisticated presence.

For technical readouts, telemetry, and system labels, **Geist** is used to provide a monospaced, precise feel that suggests engineering accuracy. All caps with increased letter spacing should be applied to `label-sm` to ensure legibility against blurred glass backgrounds.

## Layout & Spacing
The layout follows a **Fluid Grid** philosophy, allowing the "Smart Glass" panels to expand and contract like the views from a yacht's deck. We employ a 12-column grid for desktop, but the primary differentiator is the "Airy Margin"—large, breathable gaps between interactive zones to prevent the UI from feeling cluttered.

On mobile and tablet bridge-controls, margins are fixed to `24px` to ensure touch targets remain clear. Content should be grouped into "Instructional Clusters," where related environmental controls (Tint, Temperature, Opacity) are separated by significant whitespace to allow the background maritime environment to remain visible through the interface.

## Elevation & Depth
Depth is not achieved through shadows, but through **Optical Refraction**. We use three distinct layers of "Glass":

1.  **Base Layer:** The yacht's live view or a deep navy gradient.
2.  **Mid Layer (Plates):** Translucent cards with a `20px` to `40px` backdrop-blur. These use a 1px "Polished" border—a subtle white-to-transparent linear gradient that mimics light hitting the edge of a glass pane.
3.  **Top Layer (Interactions):** Active buttons or focused modals use a secondary "Azure Glow" (`00A3FF` at 15% opacity) behind the glass to indicate presence and elevation.

Avoid drop shadows entirely. Use `backdrop-filter: blur()` and `border: 1px solid rgba(255,255,255,0.1)` to define boundaries.

## Shapes
The shape language is "Soft-Geometric." While the architecture of a yacht is often aerodynamic and curved, the interface uses consistent `rounded-lg` (16px) and `rounded-xl` (24px) corners to balance modern tech with organic fluidity. 

Interactive elements like buttons use the `rounded-xl` setting to feel approachable and tactile, while container cards use `rounded-lg` to maintain a sense of structural integrity.

## Components
- **Glass Cards:** The primary container. Must have a `backdrop-filter: blur(24px)`, a background of `rgba(255,255,255,0.03)`, and a 1px border.
- **Action Buttons:** Fully transparent with a thick Azure border or solid Azure with high transparency. Text should always be white for maximum contrast.
- **Environmental Sliders:** Used for glass tinting and lighting. The track should be a thin white line; the "thumb" should be a glowing Azure circle that leaves a soft light trail.
- **Status Chips:** Small, pill-shaped glass elements with a "Pulse" dot. A green pulse for "Clear," an Azure pulse for "Smart-Tint Active."
- **Data Lists:** No dividers. Use increased vertical padding (`16px`) and subtle background hover states that slightly increase the glass opacity.
- **Segmented Controls:** Designed to look like a single pane of glass etched with dividers. The "Selected" state is a soft Azure inner glow.
- **Telemetry Gauges:** Circular, thin-stroke displays for wind speed and glass temperature, using the primary Azure color for the progress arc.