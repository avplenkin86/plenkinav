---
name: Architectural Integrity
colors:
  surface: '#0b141c'
  surface-dim: '#0b141c'
  surface-bright: '#313a43'
  surface-container-lowest: '#060f17'
  surface-container-low: '#131d24'
  surface-container: '#172128'
  surface-container-high: '#212b33'
  surface-container-highest: '#2c363e'
  on-surface: '#dae4ef'
  on-surface-variant: '#c3c5d9'
  inverse-surface: '#dae4ef'
  inverse-on-surface: '#28313a'
  outline: '#8d90a2'
  outline-variant: '#434656'
  surface-tint: '#b6c4ff'
  primary: '#b6c4ff'
  on-primary: '#00277f'
  primary-container: '#0057ff'
  on-primary-container: '#e5e8ff'
  inverse-primary: '#004ee7'
  secondary: '#c6c6ca'
  on-secondary: '#2f3034'
  secondary-container: '#4a4b4f'
  on-secondary-container: '#bbbbbf'
  tertiary: '#c2c7cd'
  on-tertiary: '#2c3136'
  tertiary-container: '#64696f'
  on-tertiary-container: '#e5e9f0'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b6c4ff'
  on-primary-fixed: '#001550'
  on-primary-fixed-variant: '#003ab2'
  secondary-fixed: '#e2e2e6'
  secondary-fixed-dim: '#c6c6ca'
  on-secondary-fixed: '#1a1c1f'
  on-secondary-fixed-variant: '#45474a'
  tertiary-fixed: '#dee3e9'
  tertiary-fixed-dim: '#c2c7cd'
  on-tertiary-fixed: '#171c21'
  on-tertiary-fixed-variant: '#42474d'
  background: '#0b141c'
  on-background: '#dae4ef'
  surface-variant: '#2c363e'
typography:
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: 0em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
  code:
    fontFamily: monospace
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
spacing:
  unit: 4px
  gutter: 24px
  margin: 64px
  container-max: 1440px
  grid-subtle-opacity: '0.05'
---

## Brand & Style

The design system is rooted in the philosophy of "Architectural Integrity," translating the precision of structural engineering into a digital portfolio. It targets high-stakes stakeholders—CTOs, Founders, and Engineering VPs—evoking feelings of reliability, intellectual depth, and technical mastery. 

The style is **Minimalist-Structural**. It leverages heavy whitespace and a strict mathematical grid to create a sense of organized complexity. Unlike standard corporate minimalism, this system uses thin, visible guide-lines and data-heavy layouts to mimic a blueprint. The aesthetic bridges the gap between the grounded history of software engineering and the forward-thinking nature of AI-driven systems.

## Colors

The palette is anchored in a professional Dark Mode to emphasize focus and technical sophistication.
- **Primary (Electric Blueprint):** A high-vibrancy blue used exclusively for interactive elements, data visualization peaks, and primary calls to action. It represents the "spark" of innovation.
- **Secondary (Obsidian):** The foundation. A deep, near-black slate used for the primary background to reduce eye strain and provide infinite depth.
- **Tertiary (Structural Gray):** Used for card backgrounds and section dividers. It provides a subtle lift from the background.
- **Neutral (Concrete & Silver):** A range of cool grays used for secondary text and non-essential structural lines, ensuring a clear hierarchy of information.

## Typography

This design system utilizes a high-contrast typographic pairing to signal both technical innovation and functional readability. 
- **Space Grotesk** is used for headlines and UI labels. Its geometric, slightly "tech" quirks provide a futuristic edge suitable for an architect working with modern AI stacks.
- **Inter** is the workhorse for body copy. It is chosen for its exceptional legibility at small sizes and its neutral, systematic feel.
- **Caps & Spacing:** Small labels and metadata should use uppercase with increased letter spacing to mimic the annotations found on architectural drawings.

## Layout & Spacing

The layout is a **Fixed 12-Column Grid** centered within the viewport. 
- **The "Blueprint" Overlay:** A subtle background grid (using the `grid-subtle-opacity`) should be visible across the entire canvas, acting as a canvas for the UI.
- **Structural Lines:** Use 1px solid lines (color: Tertiary) to separate major sections. These lines should extend to the edges of the viewport where possible, reinforcing the "unending grid" concept.
- **Rhythm:** All margins and paddings must be multiples of 8px. Use generous vertical spacing (80px+) between major sections to allow the content to breathe and signify importance.

## Elevation & Depth

This system rejects traditional soft shadows in favor of **Layered Structuralism**.
- **Tonal Elevation:** Depth is achieved by shifting background colors. The base is Obsidian (#121417), and elevated surfaces (cards, modals) use Structural Gray (#24292E).
- **Low-Contrast Outlines:** Instead of shadows, use 1px borders for all containers. These borders should be slightly lighter than the surface they contain.
- **Focus States:** When an element is active or hovered, use the Primary Accent color for the border or a subtle outer glow with 0 blur, maintaining the "sharp" technical aesthetic.

## Shapes

To maintain the "Architectural Integrity" theme, the system uses **Sharp (0px) corners** for almost all UI elements. This conveys precision, rigidity, and a "no-frills" engineering mindset. 

Roundedness is only permitted in specific AI-driven data visualizations or circular status indicators to provide a visual contrast between "Structural" (the system) and "Organic" (the data/intelligence).

## Components

- **Buttons:** Rectangular with no radius. Primary buttons use a solid Blueprint Blue fill with white text. Secondary buttons use a ghost style (1px border) with an "X" or "L-bracket" corner detail to mimic drafting marks.
- **Cards:** Defined by 1px borders. Use "Coordinate" labels in the top-right corner of cards (e.g., SECTION_01 // REF_44) in the `label-caps` style to enhance the blueprint theme.
- **Input Fields:** Bottom-border only by default. On focus, the border shifts to the Primary color and a subtle vertical line appears at the start of the label.
- **Chips/Tags:** Small, rectangular containers with the `label-caps` font. They should look like metadata tags on a schematic.
- **Diagrams:** Use thin lines, arrows with open heads, and monospace annotations. 
- **Navigation:** A persistent, minimal sidebar or top bar that uses vertical lines to separate links, reminiscent of a ruler or scale.