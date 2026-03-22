---
name: selfdriven-ecosystem-visual
description: >
  Create selfdriven Foundation branded explanatory graphics, diagrams, timeline illustrations,
  and conceptual visuals as standalone HTML/SVG artifacts. Use this skill whenever the user
  wants to produce an image, chart, infographic, diagram, timeline, or visual explainer in
  the selfdriven visual style — including situational awareness diagrams, progression charts,
  framework visuals, AI capability timelines, and any branded one-pager graphic. Trigger even
  if the user says "make an image", "create a visual", "diagram this", or "illustrate this"
  in a selfdriven context. Always use this skill instead of generic chart libraries when the
  output needs selfdriven brand fidelity.
---

# selfdriven Ecosystem Image Creator

Produce branded explanatory graphics and visual diagrams for the selfdriven Foundation ecosystem.
Output is always a **self-contained HTML file** that renders at 1600×900px (landscape) or
1200×800px (portrait/square) and can be screenshotted or printed to an image.

---

## Brand System (Image-Specific)

### Colour Palette

```
Background:         #F0ECE5   (warm linen — page/canvas ground)
Surface dark:       #3D3B38   (charcoal pill / label callout)
Surface mid:        #C8BFB0   (subtle secondary surface)
Surface light:      #E8E2D8   (divider / muted band)

Accent — Flamingo:  #C8442F   (selfdriven primary red; Level 1 / "Legacy" / danger)
Accent — Amber:     #E8732A   (transitional / warm mid-state; Level 2 / "Transitional")
Accent — Sage:      #4A7C59   (positive / resolved / forward; Level 3 / "Now" / green)
Accent — Lavender:  #B8A8D0   (background for callout pills; "Tools That Can Make Decisions")
Accent — Indigo:    #5A4A8A   (deep purple text on lavender surfaces)

Text primary:       #1A1410   (near-black warm)
Text secondary:     #6B5F52   (warm mid-grey)
Text inverse:       #F0ECE5   (on dark surfaces)
```

### Typography

- **Display / headline**: `Poppins`, weight 800–900, letter-spacing -0.03em
- **Subhead / label**: `Poppins`, weight 600–700
- **Body / descriptor**: `Poppins`, weight 400–500
- **Monospace / technical**: `JetBrains Mono`
- **Load from Google Fonts**: `https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;600&display=swap`

### Visual Language

| Element | Treatment |
|---|---|
| Level badges | Large filled circle (60–80px), bold white number, colour = level accent |
| Sub-badges | Small circle (28px) with letter (A/B), white ring, sits adjacent to parent |
| Horizontal timelines | Thick horizontal bar (4–6px), capped with flat terminator, coloured per level |
| Dashed arrow | `stroke-dasharray: 8 5`, animated `stroke-dashoffset` for motion feel |
| Callout pills (dark) | Rounded rect `#3D3B38`, white headline + muted subtitle, 24px radius |
| Callout pills (light) | Rounded rect lavender `#B8A8D0`, indigo `#5A4A8A` headline |
| Column dividers | 1.5px solid `#B0A898`, full height |
| Background texture | Diagonal hatching lines (SVG `pattern`), very low opacity (0.04–0.07), top-right decorative |
| Logo | selfdriven wordmark bottom-right, `color: #C8442F`, Poppins 700, with lightning-bolt SVG mark |

---

## Diagram Types

### 1. Horizontal Timeline / Progression Chart

This is the primary selfdriven diagram format (see "A Moment in Human History" reference).

**Structure:**
- Canvas: `1600×900` landscape HTML
- Column layout: 3–4 vertical time-bands separated by column dividers
- Each column has a header label (`Before YYYY`, `After YYYY`, etc.) and large year text
- Horizontal bars span across columns per level/row
- Bars are terminated with a flat `|` cap at their endpoint
- Level circles sit at the origin of each bar, left-aligned
- A dashed arrow from transitional level downward indicates trajectory/future state
- Callout pills float left (dark surface for upper level) and centre-right (light/lavender for emerging level)
- Row labels below bars: italic, small, warm mid-grey (`Human In Control`, `Machine In Control`, etc.)

**Grid proportions:**
```
Canvas: 1600 × 900px
Left margin (label col): ~160px
Column 1 (Before 2022): ~320px
Column 2 (After 2023): ~340px  
Column 3 (After 2025): ~780px
Top padding: 60px
Row spacing: ~180px per level tier
```

### 2. Framework Grid

3 or 4-column card grid illustrating 8 Areas of Focus or framework components.

- Cards: `20px` radius, `1px solid #DDD8CE`, accent top-bar `3px #C8442F`
- Number badge: `28px` circle, flamingo fill, white number
- Hover: subtle lift shadow

### 3. Flow / Process Diagram

Vertical or horizontal step sequence with numbered connectors.

- Step nodes: rounded rect, accent-coloured outline
- Connectors: `→` or `↓` with label
- Branching: dashed line for conditional paths

### 4. Comparison / Before-After

Two-panel layout with contrast shading.

- Left panel: `#E8E2D8` surface — "before" / legacy state
- Right panel: `#C8442F` or `#4A7C59` accent — "after" / new state
- Divider: diagonal cut or clean vertical line

---

## HTML Scaffold

Always produce a **single self-contained HTML file**. No external JS dependencies beyond Google Fonts.

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=1600">
<title>[Diagram Title] — selfdriven</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body {
    width: 1600px; min-height: 900px;
    background: #F0ECE5;
    font-family: 'Poppins', sans-serif;
    color: #1A1410;
    overflow: hidden;
    position: relative;
  }
  /* ... diagram-specific styles ... */
</style>
</head>
<body>
  <!-- Diagram content here -->
  <!-- selfdriven logo bottom-right -->
  <div class="sd-logo">
    <svg ...><!-- lightning bolt mark --></svg>
    <span>selfdriven</span>
  </div>
</body>
</html>
```

---

## selfdriven Logo Mark (SVG)

Use this inline SVG for the selfdriven lightning-bolt wordmark in the bottom-right corner:

```svg
<svg width="18" height="22" viewBox="0 0 18 22" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M10.5 1L1 13H9L7.5 21L17 9H9L10.5 1Z"
        fill="#C8442F" stroke="#C8442F" stroke-width="1.2"
        stroke-linejoin="round"/>
</svg>
```

Logo lockup CSS:
```css
.sd-logo {
  position: absolute;
  bottom: 32px; right: 40px;
  display: flex; align-items: center; gap: 8px;
  font-family: 'Poppins', sans-serif;
  font-weight: 700; font-size: 17px;
  color: #C8442F;
  letter-spacing: -0.01em;
}
```

---

## Situational Awareness Level System

When building AI capability / human-machine control diagrams, use this canonical level system:

| Level | Name | Colour | Badge | Description |
|---|---|---|---|---|
| 1 | Legacy | `#C8442F` (flamingo) | Red circle `1` | Humans totally control the tools; all decisions by humans |
| 2 | Transitional | `#E8732A` (amber) | Orange circle `2` with sub-badges `A` / `B` | Human & machine share control; ChatGPT era |
| 3 | Machine in Control / Human in Context | `#4A7C59` (sage green) | Green circle `3` | Machine makes decisions; machine understands humans more than humans understand machine |

### Sub-level Badges (Level 2)
- **2A**: AI as tool (human-initiated, human-confirmed)
- **2B**: AI as agent (human-delegated, machine-executed)

### Timeline Periods
- Before 2022 → Level 1 dominant
- After 2023 → Level 2 emerges (2A then 2B)
- After 2025 / Jan 2026 → Level 3 emergence
- "Now" arrow on Level 3 points right (open-ended, ongoing)

---

## Callout Pill Patterns

### Dark Pill (upper/legacy state)
```html
<div class="pill-dark">
  <div class="pill-title">Humans Totally Control The Tools</div>
  <div class="pill-sub">We made all the decisions</div>
</div>
```
```css
.pill-dark {
  background: #3D3B38;
  border-radius: 20px;
  padding: 28px 40px;
  color: #F0ECE5;
}
.pill-dark .pill-title { font-size: 36px; font-weight: 800; }
.pill-dark .pill-sub { font-size: 16px; color: #B0A898; margin-top: 6px; }
```

### Lavender Pill (emerging/future state)
```html
<div class="pill-lavender">
  <div class="pill-title">Tools That Can Make Decisions</div>
  <div class="pill-sub">Machine understands humans more than humans understand the machine</div>
</div>
```
```css
.pill-lavender {
  background: #B8A8D0;
  border-radius: 24px;
  padding: 36px 48px;
  color: #2A1F4A;
}
.pill-lavender .pill-title { font-size: 40px; font-weight: 800; color: #1A1060; }
.pill-lavender .pill-sub { font-size: 16px; color: #4A3A6A; margin-top: 10px; max-width: 380px; line-height: 1.5; }
```

---

## Background Texture (Diagonal Hatching)

Add decorative diagonal lines in top-right corner for depth:

```html
<svg class="bg-texture" width="600" height="500" ...>
  <defs>
    <pattern id="hatch" width="20" height="20" patternTransform="rotate(30)" patternUnits="userSpaceOnUse">
      <line x1="0" y1="0" x2="0" y2="20" stroke="#6B5F52" stroke-width="0.8" opacity="0.15"/>
    </pattern>
  </defs>
  <rect width="600" height="500" fill="url(#hatch)"/>
</svg>
```

Position: `position: absolute; top: 0; right: 0; opacity: 0.4; pointer-events: none;`

---

## Dashed Animated Arrow (Trajectory)

For showing transitional trajectory / emerging path:

```html
<svg class="trajectory-arrow" ...>
  <line x1="..." y1="..." x2="..." y2="..."
        stroke="#E8732A" stroke-width="3"
        stroke-dasharray="10 6"
        stroke-linecap="round"/>
  <!-- arrowhead -->
  <polygon points="..." fill="#E8732A"/>
</svg>
```

Optional CSS animation:
```css
@keyframes dash { to { stroke-dashoffset: -32; } }
.trajectory-arrow line { animation: dash 1.2s linear infinite; }
```

---

## Column / Row Label System

```
Column headers:     Poppins 500, 14px, #6B5F52, uppercase tracking 0.08em
Year display:       Poppins 800, 64–80px, #1A1410, letter-spacing -0.04em
Column note:        Poppins 400, 13px, #9E9085, italic  e.g. "(Jan 2026)"
Row level labels:   Poppins 500, 13px, #6B5F52  e.g. "Human In Control"
Level name labels:  Poppins 600, 15px, colour = level accent  e.g. "Legacy", "Transitional", "Now"
```

---

## Output Checklist

Before delivering an image artifact:

- [ ] Canvas is `1600×900` (landscape) or `1200×800` (portrait)
- [ ] Background is warm linen `#F0ECE5`, not white
- [ ] Poppins font loaded from Google Fonts
- [ ] selfdriven logo lockup in bottom-right (lightning bolt + "selfdriven" in flamingo)
- [ ] Level colours are correct: Red=1, Amber=2, Green=3
- [ ] Callout pills use correct dark (`#3D3B38`) or lavender (`#B8A8D0`) surfaces
- [ ] Diagonal texture in top-right corner at low opacity
- [ ] Column dividers are `#B0A898` 1.5px
- [ ] No white backgrounds on any surface element
- [ ] Year labels are Poppins 800 large and bold
- [ ] Dashed arrow is amber `#E8732A` with correct dasharray
- [ ] `overflow: hidden` on body to prevent scroll artifacts
