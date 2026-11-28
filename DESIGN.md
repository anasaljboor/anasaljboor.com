---
name: Anas Al-Jboor
description: Software engineer and DevOps engineer. Wayfinding signage on sand, one burnt-orange line.
colors:
  sand: "#f6f2ea"
  paper: "#fffdf8"
  ink: "#1b1712"
  ink-2: "#3b342b"
  muted: "#6a6152"
  rule: "#d9d0bf"
  line: "#c2410c"
  line-hi: "#a3360a"
  on-line: "#ffffff"
  band: "#1b1712"
  band-text: "#f6f2ea"
  band-body: "#e4dccd"
  band-muted: "#bdb19c"
  band-rule: "#3d362d"
  ok: "#2f7d4f"
  err: "#b42318"
typography:
  display:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(46px, 6.4vw, 92px)"
    fontWeight: 800
    lineHeight: 0.96
    letterSpacing: "-0.035em"
  display-terminus:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(44px, 6vw, 80px)"
    fontWeight: 800
    lineHeight: 0.96
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(34px, 4.2vw, 54px)"
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: "-0.03em"
  figure:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "44px"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.03em"
    fontFeature: "tnum"
  title:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "23px"
    fontWeight: 800
    lineHeight: 1.15
    letterSpacing: "-0.015em"
  lede:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(19px, 1.6vw, 22px)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
    fontFeature: "tnum"
  label:
    fontFamily: "Overpass, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 600
    lineHeight: 1.4
rounded:
  sm: "4px"
  full: "50%"
spacing:
  xs: "8px"
  sm: "14px"
  md: "28px"
  lg: "40px"
  xl: "64px"
  section: "96px"
  section-mobile: "64px"
  gutter: "24px"
  gutter-mobile: "16px"
  wrap: "1180px"
  dot: "26px"
  bar: "8px"
components:
  button-primary:
    backgroundColor: "{colors.line}"
    textColor: "{colors.on-line}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "14px 20px"
  button-primary-hover:
    backgroundColor: "{colors.line-hi}"
    textColor: "{colors.on-line}"
  button-small:
    backgroundColor: "{colors.line}"
    textColor: "{colors.on-line}"
    rounded: "{rounded.sm}"
    padding: "9px 14px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "14px 20px"
  button-ghost-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.band-text}"
  button-ink:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.band-text}"
    rounded: "{rounded.sm}"
    padding: "14px 20px"
  nav-band:
    backgroundColor: "{colors.band}"
    textColor: "{colors.band-text}"
    height: "60px"
  monogram:
    backgroundColor: "{colors.line}"
    textColor: "{colors.on-line}"
    rounded: "{rounded.full}"
    size: "30px"
  station-dot:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.full}"
    size: "{spacing.dot}"
  input:
    backgroundColor: "{colors.sand}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "12px 14px"
  input-focus:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
  form-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "32px"
  terminal-band:
    backgroundColor: "{colors.line}"
    textColor: "{colors.on-line}"
---

# Design System: Anas Al-Jboor

## Overview

**Creative North Star: "The Line"**

The site is a piece of wayfinding signage. A sand ground carries ink signage bands with sand lettering, and through it runs one thick burnt-orange line with white stations ringed in ink. The work Anas covers (interface, API and data, cloud and CI/CD, search) is drawn as stops on that line, and the line ends at a terminus: the client's launch, and at the foot of the page, an orange section where the visitor books a call. The line runs horizontally on wide screens and turns vertical below 920px, the way a route map is redrawn for a narrow panel.

Everything is set in one face, Overpass, a descendant of the Highway Gothic lettering on road signs, at three weights. Times and figures use tabular numerals, so the services read as a timetable. Surfaces are flat. Structure comes from rules (2px ink rules open a group, 1px sand rules divide rows), from full-bleed colour bands, and from the line itself. Corners are square-ish at 4px; the only round forms are the stations and the monogram.

The world explicitly refuses the split hero with a floating gradient card, icon-tile service cards and code-chip decoration. There are no gradients, no drop shadows, no glass and no monospace.

**Key Characteristics:**
- One burnt-orange line (8px bar) with 26px stations: paper fill, 5px ink ring.
- Ink bands (nav, recruiter section, footer) with sand text; one orange terminus band for contact.
- Overpass only, weights 400 / 600 / 800, tabular figures throughout.
- Flat surfaces, 4px corners, structure carried by 2px ink and 1px sand rules.
- Timetable rows instead of cards.

## Colors

A warm sand-and-ink signage palette with a single saturated line colour that carries every action and the route itself.

### Primary
- **Burnt Orange Line** (`line`): the route bar, every primary button, link underlines, the focus outline, the FAQ plus sign, text selection, the monogram disc, and the full-bleed contact terminus. It is the only chromatic colour on the page.
- **Deep Line** (`line-hi`): hover state of primary buttons.
- **White on Line** (`on-line`): text and icons set on the line colour.

### Neutral
- **Sand** (`sand`): the page ground; also input fields at rest.
- **Paper** (`paper`): station fills, the contact form card, focused inputs. One step lighter than sand, never a raised card.
- **Ink** (`ink`): body text, headings, station rings, 2px group rules, ghost button borders.
- **Ink Soft** (`ink-2`): lede, descriptions and list items under a heading.
- **Muted Earth** (`muted`): secondary notes, stacks, metadata, column heads.
- **Sand Rule** (`rule`): 1px row dividers and input borders at rest.
- **Signage Band** (`band`, same value as ink): nav, recruiter section, footer, the hero portrait caption.
- **Band Sand** (`band-text`), **Band Body** (`band-body`), **Band Muted** (`band-muted`), **Band Rule** (`band-rule`): heading, body, secondary and divider colours on the ink band.

### Status
- **Signal Green** (`ok`) and **Signal Red** (`err`): form status messages and invalid field borders only.

### Named Rules
**The One Line Rule.** Burnt orange belongs to the line and to what moves the visitor along it: the route, actions, links, focus. It never becomes a decorative fill, a tint wash or a gradient.

**The Signage Band Rule.** Full-bleed colour bands are the only way to change ground. Ink bands carry sand text; the single orange band is the terminus and holds the contact paths. No third band colour.

## Typography

**Display Font:** Overpass (with Helvetica Neue, Arial, sans-serif)
**Body Font:** Overpass
**Label Font:** Overpass

**Character:** Highway-sign lettering used for every word, so the page reads as one piece of signage. Hierarchy comes from size and the jump between 400, 600 and 800, never from a second family.

### Hierarchy
- **Display** (800, clamp(46px, 6.4vw, 92px), 0.96, -0.035em): the hero H1 only, held to about 11.5em wide.
- **Display Terminus** (800, clamp(44px, 6vw, 80px), 0.96): the contact heading and the 404 heading.
- **Headline** (800, clamp(34px, 4.2vw, 54px), 1.02, -0.03em): section H2s. A 30px 800 sub-head splits a section in two.
- **Figure** (800, 44px, 1, tabular): typical times in the timetable; 32px below 920px.
- **Title** (800, 19-25px, 1.15, -0.015em): station names (21px), service names (23px), case titles (25px), project names (19px).
- **Lede** (400, clamp(19px, 1.6vw, 22px), 1.45): the hero paragraph, max 34em. Section subs sit at 19px muted, max 44em.
- **Body** (400, 17px, 1.55): running text, max about 44em; 15-16px for notes and lists.
- **Label** (600, 15px): nav links, form labels, column titles, buttons (16px). Sentence case, no tracking.

### Named Rules
**The One Face Rule.** Overpass sets every word, including figures and the form. No monospace, no serif, no second display face.

**The Timetable Figure Rule.** Numbers are tabular everywhere (`font-variant-numeric: tabular-nums` on body), and a time is set large in 800 with its unit beside it at body size.

## Layout

A single centred wrap (1180px, 24px side gutters; 16px below 640px). Sections are full width with 96px vertical padding (64px on phones), separated by a 1px sand rule unless the next section is a colour band. A section head (H2 plus muted sub, max 760px) sits 48px above its content.

The hero is a two-column grid: copy across the left, a 300px portrait with an ink signage caption on the right, aligned to the bottom. Under it the horizontal line spans the full wrap: four stations in equal columns and a wider terminus column (1.35fr) holding the primary call and two text links. Services form a three-column timetable (name and summary, what you get, typical time) on a vertical line. Work entries are two-column rows (where and when, then what was built), and side projects are a three-column list. The FAQ is a 1fr / 2fr split.

Responsive behaviour: at 1080px the timetable columns narrow; at 920px the nav links hide (brand and the small CTA remain), every horizontal line turns vertical with stations at the left, the timetable collapses to one column with the time inline, and two-column splits stack; at 640px the portrait becomes a 96px square beside its caption, hero buttons go full width and a mobile booking button appears under the lede.

Gaps step through 8, 14, 28, 40, 56 and 64px.

### Named Rules
**The Route Turns Rule.** A line diagram is horizontal only while every stop gets a readable column; below 920px it is redrawn vertically, never shrunk or scrolled sideways.

## Elevation & Depth

Flat. There are no drop shadows and no blur. Depth is conveyed by ground changes (sand to ink band to orange terminus), by the one-step lift from sand to paper on the form card and stations, and by rules. The only `box-shadow` in the system is a spread-only double ring that marks the terminus station.

### Shadow Vocabulary
- **Terminus ring** (`box-shadow: 0 0 0 5px var(--bg), 0 0 0 8px var(--ink)`): a sand gap and an outer ink ring around a solid ink station, the interchange symbol of a route map. Used only on the final stop of a line.

### Named Rules
**The Flat Signage Rule.** Nothing floats. If a surface needs separation, give it a rule or a band, not a shadow. Spread-only rings on stations are the one exception, because they are part of the map's symbol set.

## Shapes

Square-ish 4px corners on buttons, inputs, the form card, the portrait and its caption (the photo rounds only on the top, the caption only on the bottom, so the two read as one sign). Circles are reserved for stations. The logo is text only; the favicon is sand "AA" on an ink square with an orange underline bar. The line bar is a capsule (radius equal to its 8px thickness). List bullets are 7px solid ink squares. Rules come in two weights: 2px ink opens a group (timetable head, case, FAQ item, band column title), 1px sand divides rows.

## Components

### Buttons
Solid, plain and signage-like: a filled rectangle with a label and an optional 18px stroke icon.
- **Shape:** 4px corners, 2px border in the fill colour.
- **Primary:** line fill, white text, 600 16px, 14px 20px padding, 10px icon gap.
- **Hover / Active:** fill and border shift to deep line over .18s; active nudges down 1px.
- **Small:** 9px 14px, 15px text; the nav CTA.
- **Ghost:** transparent with a 2px ink border and ink text; hover fills ink with sand text. On the ink band it inverts to sand border and text.
- **Ink:** ink fill with sand text, used on the orange terminus where an orange button would vanish.
- **Disabled:** 60% opacity, progress cursor.

### Text links
600 weight, 2px burnt-orange underline offset 5px; hover turns the text orange. Inline links in case stacks and FAQ answers use the same underline. Contact channels on the orange band use a 1px white underline that thickens to 2px on hover.

### Navigation
A sticky 60px ink band. Text-only wordmark "Anas Al-Jboor" (Overpass 800, 20px, -0.02em) at left, sand-muted 600 15px links that brighten to sand on hover, an outlined "CV" button and the small primary CTA at right. Below 920px only brand and CTA remain.

### Inputs / Fields
- **Style:** sand fill, 2px sand-rule border, 4px corners, 12px 14px padding, 400 16px text; label above in 600 15px with optional hints in muted 400.
- **Hover:** border darkens to a mid sand.
- **Focus:** border goes ink and the fill lifts to paper; no glow.
- **Error:** after a submit attempt, invalid fields take the red border; status text below in red or green.

### Form card
A paper panel (32px padding, 4px corners) set on the orange terminus band, holding the contact form. It is the one boxed surface on the page.

### Line and stations (signature)
An 8px burnt-orange capsule behind a row (or column) of 26px stations: paper fill, 5px ink ring. Each station has an 800 21px name and a muted 15px one-line note. Hovering a station's link fills it orange, scales it to 1.12 and underlines the name in 3px orange. The terminus station is solid ink with the sand-gap ring. On load, the hero line draws left to right once (1.2s, clip-path) when motion is allowed.

### Timetable row (signature)
A service on the vertical line: station at left, then name and summary, a square-bulleted list of what is included, and the typical time in 44px tabular 800 with "Fixed quote after a call" below in muted 14px. A 2px ink head row labels the columns; 1px sand rules divide rows.

### Signage band
Full-bleed ink section for recruiters: sand headings, band-body text, columns opened by a sand 2px rule under a 600 15px column title, rows divided by band-rule lines.

### FAQ item
A disclosure opened by a 2px ink rule, 600 20px question, and a 3px orange plus sign that rotates 45 degrees to a cross when open.

## Do's and Don'ts

### Do:
- **Do** route every primary action through burnt orange (`line`) and keep orange off anything that is not the route, an action, a link or focus.
- **Do** draw sequences (scope, process, services) as stations on the line, horizontal above 920px and vertical below.
- **Do** set every word in Overpass at 400, 600 or 800, with tabular figures.
- **Do** separate content with 2px ink rules for groups and 1px sand rules for rows, and change ground only with a full-bleed band.
- **Do** keep corners at 4px and reserve circles for stations.
- **Do** use a 3px burnt-orange focus outline offset 3px (ink on the orange band, sand on the ink band).

### Don't:
- **Don't** use gradients, drop shadows, glass or blur; the terminus ring is the only `box-shadow`.
- **Don't** build a split hero with a floating gradient card, icon-tile service cards or code-chip decoration.
- **Don't** introduce monospace or a second typeface.
- **Don't** add a second chromatic accent or a third band colour.
- **Don't** wrap services or work in cards; they are rows on a line or under a rule.
