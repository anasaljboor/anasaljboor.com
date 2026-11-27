---
name: Anas Al-Jboor
description: One engineer, the whole path. A dark offer page with one warm yellow voice.
colors:
  bg: "#0c0c0d"
  panel: "#151517"
  panel-2: "#1b1b1e"
  line: "#262629"
  line-2: "#3a3a3f"
  fg: "#f3f3f2"
  fg-soft: "#cfcfd2"
  muted: "#a3a3a9"
  accent: "#ffc83d"
  accent-hi: "#ffd666"
  accent-ink: "#1a1400"
  accent-wash: "rgba(255, 200, 61, .1)"
  accent-edge: "rgba(255, 200, 61, .28)"
  amber-edge: "#3a3112"
  ok: "#3ddc84"
  err: "#ff8a7a"
typography:
  display:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "clamp(40px, 5.6vw, 68px)"
    fontWeight: 800
    lineHeight: 1.04
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "clamp(28px, 3.4vw, 40px)"
    fontWeight: 700
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "21px"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.02em"
  lede:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "19px"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "13.5px"
    fontWeight: 400
    lineHeight: 1.5
  mono:
    fontFamily: "JetBrains Mono, ui-monospace, Menlo, monospace"
    fontSize: "12px"
    fontWeight: 400
rounded:
  code: "7px"
  chip: "8px"
  sm: "10px"
  md: "12px"
  card: "18px"
  feature: "22px"
  stage: "24px"
  full: "50%"
spacing:
  gutter: "24px"
  gutter-mobile: "16px"
  gap: "16px"
  card-pad: "28px"
  section: "72px"
  section-mobile: "56px"
  container: "1120px"
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.accent-ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: "13px 20px"
  button-primary-hover:
    backgroundColor: "{colors.accent-hi}"
    textColor: "{colors.accent-ink}"
  button-ghost:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.fg}"
    rounded: "{rounded.md}"
    padding: "13px 20px"
  button-small:
    rounded: "{rounded.sm}"
    padding: "8px 14px"
  card:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.fg}"
    rounded: "{rounded.card}"
    padding: "{spacing.card-pad}"
  card-chosen:
    backgroundColor: "{colors.accent-wash}"
    textColor: "{colors.fg}"
    rounded: "{rounded.card}"
    padding: "26px 28px"
  input:
    backgroundColor: "rgba(0, 0, 0, .35)"
    textColor: "{colors.fg}"
    rounded: "{rounded.md}"
    padding: "12px 14px"
  icon-tile:
    backgroundColor: "{colors.accent-wash}"
    textColor: "{colors.accent}"
    rounded: "{rounded.md}"
    size: "44px"
  nav:
    backgroundColor: "rgba(12, 12, 13, .82)"
    textColor: "{colors.muted}"
    height: "64px"
  code-chip:
    backgroundColor: "rgba(0, 0, 0, .35)"
    textColor: "{colors.ok}"
    typography: "{typography.mono}"
    rounded: "{rounded.code}"
    padding: "4px 9px"
---

# Design System: Anas Al-Jboor

## Overview

**Creative North Star: "The Lit Path"**

A near-black workshop with one lamp on. Everything sits on a dark, faintly cool ground in hairline-bordered panels, and a single warm yellow marks what to do next and which way the work runs: the primary action, the chosen door, the line that traces interface to API to cloud to search. The yellow is the only voice that raises itself; everything else stays in greys and lets real stack names, real employers and real commands carry the page.

Density is calm and editorial rather than dashboard-tight: one idea per section, generous 72px section rhythm, left-aligned headings, body copy held to readable measures (34 to 40em). Structure comes from hairlines and rows (service rows, experience rows, FAQ rows) more than from boxed cards; cards appear where an item is a separate thing you can open. Depth is a warm amber tint rather than lift: the few panels that matter most get a gradient that starts in dark amber and fades into the panel grey.

Motion is short and purposeful: the hero copy and the path steps rise in once, the path line draws itself, hover lifts a card or button by one to three pixels and nudges its arrow. Nothing loops.

**Key Characteristics:**
- Near-black ground, grey panels, hairline borders; one warm yellow accent.
- Yellow means action or the selected path, never decoration.
- Rows and hairlines before boxes; cards only for discrete, linkable items.
- Featured panels warm up with an amber-to-panel gradient instead of shadows.
- Inter for everything readable; JetBrains Mono only for real commands.
- Line icons drawn as inline SVG at 2px stroke, rounded caps.

## Colors

A dark neutral field with a single saturated warm yellow and two small functional colors.

### Primary
- **Lamp Yellow** (accent): primary buttons, the path line and its dots, process step numbers, links inside prose, FAQ open state, focus rings, text selection. Hover brightens to **Lamp Yellow Hi** (accent-hi).
- **Lamp Ink** (accent-ink): the near-black text that sits on yellow fills (buttons, the AA monogram, selection, skip link).
- **Yellow Wash** (accent-wash) and **Yellow Edge** (accent-edge): the translucent fill and border for things in the chosen state: the client door, service icon tiles, the large portrait ring.
- **Amber Edge** (amber-edge): the solid dark-amber border on warm featured panels (the hero path, the contact block, the zero-knowledge diagram box).

### Neutral
- **Workshop Black** (bg): page ground, also the "hole" inside outlined dots and step numbers.
- **Panel Grey** (panel) and **Raised Panel** (panel-2): card and ghost-button fills; panel-2 for nested boxes inside cards and image placeholders.
- **Hairline** (line) and **Hairline Strong** (line-2): every divider and card border; line-2 is the hover border and the input border.
- **Chalk** (fg): headings and primary text. **Soft Chalk** (fg-soft): body copy inside warm panels and case studies, a step brighter than muted.
- **Ash** (muted): secondary text, nav links, metadata, descriptions.

### Functional
- **Signal Green** (ok): checkmarks in service lists, command text in code chips, form success.
- **Coral** (err): invalid fields and form errors only.

### Named Rules
**The One Lamp Rule.** Yellow is the only accent. It marks the next action or the chosen path; if an element is yellow, a visitor should be able to say what it leads to.

**The Ink-On-Lamp Rule.** Text on a yellow fill is always accent-ink, never white or fg.

## Typography

**Display Font:** Inter (with system-ui, -apple-system, Segoe UI)
**Body Font:** Inter
**Label/Mono Font:** JetBrains Mono (with ui-monospace, Menlo), for commands only

**Character:** One confident grotesque at several weights does all the talking; tight negative tracking on headings gives the page an engineered, compact voice, and mono appears only where something can literally be typed into a terminal.

### Hierarchy
- **Display** (800, clamp 40 to 68px, 1.04, -0.035em): the single hero H1.
- **Headline** (700, clamp 28 to 40px, -0.02em, balanced wrap): section titles, left-aligned, followed by a muted 17px sub line of at most 40em.
- **Title** (700, 21px, 1.25): service, case and product names. Door titles run at 22px; step and FAQ titles at 18px.
- **Lede** (400, 19px, 1.6, muted, max 34em; 17px on phones): the hero offer line.
- **Body** (400, 16px, 1.6) and **Body small** (400, 15px): running text and descriptions; most supporting copy is 15px muted.
- **Label** (400, 13 to 13.5px, muted, sentence case): metadata lines (employer, place, dates), definition terms, tags.
- **Mono** (400, 12px, Signal Green): command chips in the hero path.

### Named Rules
**The Real Command Rule.** JetBrains Mono is reserved for strings that are real commands or code (`helm upgrade --install`). Never use mono as a "techy" texture for labels or headings.

**The Sentence Case Rule.** Labels, metadata and column titles stay sentence case with no wide tracking; the system has no uppercase label style.

## Layout

A single centered column, `min(1120px, 100% - 48px)`, becoming `100% - 32px` under 640px. Sections are separated by 72px vertical padding (56px on phones) with a 32px gap between a section head and its content.

The hero is a two-column grid (1.15fr / 1fr, 56px gap) with copy left and the path panel right; it stacks at 980px. Services are full-width rows on a three-column grid (name, what's included, terms) that collapse to two columns at 980px and one at 640px. Case studies and the two entry doors use two columns; products use three; all go single-column at 980px (doors at 640px). The process is a four-step horizontal timeline on a 2px top rule, becoming 2 then 1 columns.

Breakpoints are 980px (tablet: nav links hide, grids stack) and 640px (phone: tighter gutters, primary CTAs stretch full width). Card grid gaps sit at 16 to 18px.

## Elevation & Depth

Flat by default. Depth comes from tonal steps (bg, panel, panel-2), hairline borders, and a warm amber gradient on the few panels that lead the page. There is exactly one cast shadow, under the hero path panel.

### Shadow Vocabulary
- **Path float** (`box-shadow: 0 30px 60px -20px rgba(0, 0, 0, .7)`): the hero path panel only, so it reads as the object the page is about.
- **Portrait ring** (`box-shadow: 0 0 0 2px bg, 0 0 0 4px accent` small; `0 0 0 3px bg, 0 0 0 5px accent-edge` large): a spaced ring around the portrait; a ring, not a shadow.

### Named Rules
**The Warm Glow Rule.** To make a panel feel important, warm it (a 170deg linear or top-left radial gradient from dark amber, #1d190c to #2a220a, into panel grey, with an amber-edge border), don't lift it.

**The Hover Lift Rule.** Interactive cards and buttons move 1 to 3px up on hover with a brighter border; they never gain a shadow.

## Shapes

Soft, generous rounding that scales with the size of the thing: 7 to 8px on code chips and diagram boxes, 10px on small buttons, 12px on buttons, inputs, icon tiles and logo tiles, 18px on cards, 22px on the hero path, 24px on the contact block. Circles are reserved for people and progress: the AA monogram, the portrait, path dots and step numbers. Borders are always 1px hairlines, except the 2px rules of the process timeline and the 2px outlines of path dots and step numbers.

## Components

### Buttons
Solid, compact, quietly tactile.
- **Shape:** gently rounded (12px; 10px on small buttons).
- **Primary:** yellow fill, ink text, 600 weight at 15px, 13px by 20px padding, often with a trailing arrow icon.
- **Hover / Focus:** lift 1px, primary brightens to accent-hi, the trailing icon slides 2px right; focus shows a 2px yellow outline at 3px offset. Disabled drops to 60% opacity.
- **Ghost:** panel fill with a hairline border that strengthens on hover. Used for the CV and every secondary action.
- **Small:** 8px by 14px, 14px text; the nav "Start a project" button.

### Cards / Containers
- **Corner Style:** 18px.
- **Background:** panel, hairline border; the lead items (first two case studies) take the Warm Glow gradient with an amber-edge border.
- **Shadow Strategy:** none; hover lift only (see Elevation).
- **Internal Padding:** 24 to 28px.
- **Product cards** carry a 150px visual band on #0f0f11 above the body, holding an inline SVG or box diagram of the real system, never a stock image.

### Entry doors
Two large linked panels under the hero splitting clients from recruiters. The client door is in the chosen state (yellow wash fill, yellow edge border, full yellow border on hover); the recruiter door is a plain card. Each ends in a yellow "See ..." link with an arrow.

### Inputs / Fields
- **Style:** translucent black fill (rgba(0,0,0,.35)), line-2 border, 12px radius, 12px by 14px padding, yellow caret. Labels sit above in 14px 600; optional hints in muted 400.
- **Focus:** border turns yellow and the fill deepens to rgba(0,0,0,.5); no glow.
- **Error:** after a submit attempt, invalid fields take a Coral border; status text below uses Signal Green or Coral.

### Navigation
Sticky 64px bar, 82% opaque black with a 12px backdrop blur and a hairline bottom border. AA monogram and name at left, muted 15px links that turn Chalk on hover, a small primary button at right. Under 980px the links hide and only the brand and the button remain.

### Rows
The system's main structural device: hairline-separated rows for services, experience, stack, side projects and FAQ. Experience rows lead with a 42px rounded monogram tile tinted from a per-entry hue (16% fill, 30% border); those hues belong to the entry, not the palette. FAQ rows use a drawn chevron that rotates and turns yellow when open.

### The Path (signature)
A warm-glow panel tracing the four layers of the work as a vertical timeline: a 2px yellow line that fades as it descends and draws itself on load, outlined yellow dots with the final dot filled, a 16px bold title, a muted stack line, and an optional green mono command chip. Process steps reuse its vocabulary horizontally: numbered outlined yellow circles on a 2px hairline.

### Icon tiles
44px rounded squares in yellow wash with a yellow-edge border, holding a 1.8px-stroke yellow line icon. Used once per service.

## Do's and Don'ts

### Do:
- **Do** keep yellow (#ffc83d) for actions, links and the selected path; put accent-ink text on every yellow fill.
- **Do** build structure from 1px hairlines (#262629) and rows before reaching for another card.
- **Do** warm a featured panel with the amber-to-panel gradient and an amber-edge (#3a3112) border instead of adding a shadow.
- **Do** draw icons as inline SVG line icons (24px viewBox, 2px stroke, round caps and joins) in currentColor.
- **Do** use JetBrains Mono only for real commands, set in Signal Green inside a dark code chip.
- **Do** show real systems as diagrams built from the system's own boxes and lines when no screenshot exists.
- **Do** keep entrance motion to the hero (rise, path draw) on the shared ease `cubic-bezier(.16, 1, .3, 1)`, and drop all motion under prefers-reduced-motion.

### Don't:
- **Don't** introduce a second accent hue; Signal Green and Coral are status colors, not brand colors.
- **Don't** put white or light text on yellow.
- **Don't** add drop shadows to cards or buttons; the hero path is the only floating object.
- **Don't** use uppercase, widely tracked labels, or category kickers above headings. Only factual metadata (employer, place, dates) may sit above a title, as plain sentence-case muted text.
- **Don't** use mono for labels, headings or decoration.
- **Don't** use emoji or icon fonts as icons.
