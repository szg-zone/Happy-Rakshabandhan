---
name: Kinship Audit
colors:
  surface: '#fcf9f8'
  surface-dim: '#dcd9d9'
  surface-bright: '#fcf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f0eded'
  surface-container-high: '#eae7e7'
  surface-container-highest: '#e5e2e1'
  on-surface: '#1c1b1b'
  on-surface-variant: '#4d4732'
  inverse-surface: '#313030'
  inverse-on-surface: '#f3f0ef'
  outline: '#7e775f'
  outline-variant: '#d0c6ab'
  surface-tint: '#705d00'
  primary: '#705d00'
  on-primary: '#ffffff'
  primary-container: '#ffd700'
  on-primary-container: '#705e00'
  inverse-primary: '#e9c400'
  secondary: '#b7102a'
  on-secondary: '#ffffff'
  secondary-container: '#db313f'
  on-secondary-container: '#fffbff'
  tertiary: '#5e604d'
  on-tertiary: '#ffffff'
  tertiary-container: '#dbdbc3'
  on-tertiary-container: '#5f604d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffe16d'
  primary-fixed-dim: '#e9c400'
  on-primary-fixed: '#221b00'
  on-primary-fixed-variant: '#544600'
  secondary-fixed: '#ffdad8'
  secondary-fixed-dim: '#ffb3b1'
  on-secondary-fixed: '#410007'
  on-secondary-fixed-variant: '#92001c'
  tertiary-fixed: '#e4e4cc'
  tertiary-fixed-dim: '#c8c8b0'
  on-tertiary-fixed: '#1b1d0e'
  on-tertiary-fixed-variant: '#474836'
  background: '#fcf9f8'
  on-background: '#1c1b1b'
  surface-variant: '#e5e2e1'
typography:
  audit-header-xl:
    fontFamily: Syne
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  audit-header-xl-mobile:
    fontFamily: Syne
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.1'
  stamp-label:
    fontFamily: Syne
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '500'
    lineHeight: '1.5'
  receipt-text:
    fontFamily: Courier Prime
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
  caption-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.2'
spacing:
  grid-margin: 24px
  gutter: 16px
  stack-overlap: -12px
  section-gap: 80px
---

## Brand & Style

The design system is built on the "Sister Audit" aesthetic: a collision of bureaucratic coldness and chaotic familial warmth. It targets siblings who share a language of "roasting" and nostalgia. The emotional journey moves from the anxiety of a formal performance review to the soft landing of a wholesome memory.

The style is a hybrid of **Brutalism** and **Scrapbook**. It utilizes heavy borders, monospaced data grids, and "official" stamps contrasted against grainy photo textures, digital stickers, and overlapping elements. The interface should feel like a redacted government file that has been doodled on and filled with polaroids.

## Colors

The palette is driven by high-contrast tension:
- **Primary (Audit Yellow):** A bold, warning-signal yellow used for headers and critical callouts.
- **Secondary (Rakhi Red/Pink):** A vibrant, saturated red-pink used exclusively for "Wholesome Reveal" moments, heart icons, and stickers.
- **Tertiary (Receipt Cream):** The base surface color, mimicking the look of aged thermal paper or old manila folders.
- **Neutral (Deep Black):** Used for heavy borders (3px+), typewriter text, and "Redacted" blocks.

Color application should be jarring. Transitions from the yellow/black "Audit" phase to the red/cream "Wholesome" phase should be distinct and immersive.

## Typography

Typography functions as a narrative tool. Use **Syne** for loud, expressive headlines that feel aggressive and modern. Use **JetBrains Mono** for technical data, lists, and "evidence" descriptions to maintain a structured, systematic feel. Use **Courier Prime** for the "Audit Receipt" sections to simulate a typewriter or receipt printer output.

All headers in the Audit phase should be uppercase with tight letter spacing. In the "Wholesome" phase, typography can shift to center-aligned layouts with increased whitespace to signal a change in tone.

## Layout & Spacing

This design system rejects "clean" spacing in favor of a **Layered/Overlapping** model. While a 12-column grid provides the underlying structure, elements (stickers, stamps, photos) should intentionally break the grid.

- **The Audit Phase:** Rigid, column-based, and cramped. Use heavy 4px gutters and tight margins to create a sense of information density.
- **The Wholesome Phase:** Fluid and expansive. Increase margins and use "Stack Overlap" to allow photos and stickers to lean on each other like a physical scrapbook.
- **Breakpoints:** On mobile, stack all "evidence" cards vertically but allow "Stickers" to float absolutely over text to maintain the chaotic aesthetic.

## Elevation & Depth

Avoid shadows and blurs. This design system communicates depth through **Z-index Stacking** and **Hard Outlines**:
- **Layering:** Use 2px to 4px black borders to separate surfaces. 
- **Physicality:** Elements should appear as if they are clipped or taped. Use a "Washi Tape" visual (semi-transparent colored rectangles) to "hold" images in place.
- **Textures:** Apply a global grain overlay (5-10% opacity) to the entire UI to give it a tactile, printed quality.
- **Stamps:** "Approved" or "Failed" stamps should be rotated at 15-degree increments and use a grainy, "ink-bleed" mask.

## Shapes

The primary shape language is **Sharp (0px)**. 
- **Containers:** All cards, buttons, and input fields must have 0px corner radius to reinforce the brutalist/legal-document feel.
- **Stickers:** These are the only exception. Digital stickers (stars, hearts, smiley faces) should have organic, hand-cut paths or high roundedness to contrast against the rigid UI.
- **Redaction:** Use solid black rectangles to hide "sensitive" text or as a background for high-emphasis labels.

## Components

- **Audit Cards:** Receipt-cream background, 3px solid black border, no shadow. Header in Syne Bold, content in JetBrains Mono.
- **Action Buttons:** Primary buttons are Audit Yellow with black text. On hover, they "shift" 4px down and right with a black "ghost" box remaining behind them (Neobrutalist style).
- **Evidence List:** A monospaced list where each item is prefixed with a "Case Number" (e.g., [REF-001]).
- **Digital Stickers:** Draggable (or fixed) decorative elements like "BESTIE", "CRIMINAL", or "FAIL" that can overlap other components.
- **Input Fields:** 2px black bottom-border only, using Courier Prime to look like a fill-in-the-blank form.
- **The "Verdict" Toggle:** A heavy, tactile switch that transforms the UI from the "Audit" (Yellow/Black) theme to the "Wholesome" (Red/Cream) theme using a page-wipe transition.