---
name: Teerachot Khusuwan
description: A cool, ruled page where one hue path from copper to blue plots every piece of work from hardware to web.
colors:
  ground: "oklch(98.6% 0.003 260)"
  ink: "oklch(21% 0.028 262)"
  ink-soft: "oklch(44% 0.022 262)"
  rule: "oklch(89% 0.008 262)"
  rule-strong: "oklch(78% 0.012 262)"
  range-hardware: "oklch(55% 0.14 52)"
  range-security: "oklch(51% 0.17 12)"
  range-ml: "oklch(48% 0.16 312)"
  range-web: "oklch(48% 0.16 258)"
  ink-raised: "oklch(32% 0.05 262)"
  on-ink-soft: "oklch(80% 0.015 262)"
  on-ink-rule: "oklch(45% 0.03 262)"
typography:
  display:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "clamp(3rem, 8.4vw, 6rem)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "-0.04em"
  display-contact:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "clamp(2.5rem, 6vw, 4.5rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "clamp(1.9rem, 3.6vw, 2.75rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.03em"
  lead:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "clamp(1.25rem, 2.2vw, 1.65rem)"
    fontWeight: 400
    lineHeight: 1.35
  title:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "1.3rem"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "0.85rem"
    fontWeight: 600
    lineHeight: 1.35
  small:
    fontFamily: "Schibsted Grotesk, Anuphan, system-ui, sans-serif"
    fontSize: "0.88rem"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  line: "2px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter: "clamp(20px, 4vw, 48px)"
  wrap: "1180px"
  row: "32px"
  column-gap: "40px"
  section: "clamp(72px, 11vw, 128px)"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "46px"
  button-primary-hover:
    backgroundColor: "{colors.ink-raised}"
  button-quiet:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "46px"
  lang-switch-active:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
    rounded: "{rounded.pill}"
    padding: "7px 12px"
  lang-switch-idle:
    backgroundColor: "transparent"
    textColor: "{colors.ink-soft}"
    rounded: "{rounded.pill}"
    padding: "7px 12px"
  contact-link:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "44px"
  spectrum-marker:
    backgroundColor: "{colors.ground}"
    rounded: "{rounded.circle}"
    size: "14px"
---

# Design System: Teerachot Khusuwan

## Overview

**Creative North Star: "The Range Line"**

The page is a measured drawing on cool paper. Everything is ink and hairline except one line of colour, the range, which runs copper to rose to violet to blue and plots where each piece of work sits between hardware and the web. Colour is a coordinate here, not decoration: wherever it appears, it says "this belongs at this point on the range".

Density is calm and editorial. Sections open with a large tight-set heading over a full ink rule, content sits in ruled rows and columns, and there are no cards, panels, shadows, or tinted surfaces anywhere on the light ground. The one inversion is the closing contact block, a solid ink field with the range drawn as a stripe across its top edge.

The system is bilingual by construction. Latin and Thai share one font stack, split by unicode-range, and Thai text drops negative tracking and gains leading so stacked marks never clip.

**Key Characteristics:**
- Cool near-white ground, navy-ink type, two soft ink steps for secondary text and rules.
- One four-stop hue path is the only colour, and it always encodes position on the hardware-to-web range.
- Hairline rules divide; nothing floats. No cards, no shadows.
- Pill-shaped controls; circles for markers and the monogram; everything else square.
- One load moment (the range draws, markers settle) and one linked hover (marker and work row light each other).

## Colors

A near-monochrome ink-on-paper palette carrying a single, meaningful hue path.

### Primary
- **The Range** (four stops, below): the only chromatic colour in the system. Drawn as a gradient (stops at 0%, 38%, 62%, 100%) for the spectrum line and the contact stripe; used as a single stop for band labels, marker rings, the band dot and lit rule on a work row, and a lit row's title.
  - **Copper Hardware** (range-hardware): devices and sensors, the left/top end.
  - **Signal Rose** (range-security): security work.
  - **Deep Violet** (range-ml): machine learning.
  - **Range Blue** (range-web): web and automation, the right/bottom end. Also the focus outline and text-selection tint (22% mix), the one place a range stop serves a utility role.

### Neutral
- **Cool Paper** (ground): page background, text on ink, and the hollow centre of markers.
- **Navy Ink** (ink): all primary text, the primary button, the active language pill, the monogram disc, section-head rules, and the contact/footer field.
- **Slate Ink** (ink-soft): secondary copy, nav links at rest, captions, tags, axis end labels.
- **Hairline** (rule): row dividers, column dividers, header bottom border.
- **Strong Hairline** (rule-strong): quiet-button and language-switch outlines, marker leader lines, the hero status separator, scrollbar thumb.
- **Raised Ink** (ink-raised): primary button hover only.
- **On-Ink Mist** (on-ink-soft) and **On-Ink Hairline** (on-ink-rule): secondary text and pill outlines inside the ink contact field.

### Named Rules
**The Colour Is Position Rule.** A range hue appears only on something that sits at that point on the hardware-to-web range (a band, a marker, a work row, a stripe drawing the whole range). Never use a range stop as a generic accent, status colour, or category tint for things that are not on the range. Toolkit group headings stay ink even though each group maps to a band.

**The Plain Status Rule.** Status and availability text is plain ink-soft prose. No coloured dot, badge, or pulse.

## Typography

**Display Font:** Schibsted Grotesk (variable 400 to 800, self-hosted, Latin and Latin-ext ranges)
**Body Font:** Schibsted Grotesk, same family throughout
**Thai Font:** Anuphan (variable 400 to 600, self-hosted, Thai range), next in the stack, so Thai glyphs resolve to it automatically

**Character:** One sturdy, slightly condensed grotesk does everything; hierarchy comes from size, weight, and tracking, not from a second face. Anuphan matches its plain, modern construction for Thai.

### Hierarchy
- **Display** (800, clamp 3 to 6rem, 0.95, -0.04em): the name in the hero. Balanced wrap.
- **Display Contact** (700, clamp 2.5 to 4.5rem, -0.04em): the closing contact heading on ink.
- **Headline** (700, clamp 1.9 to 2.75rem, 1.05, -0.03em): section headings. About uses a smaller clamp (1.5 to 1.9rem) because it sits in a side column.
- **Lead** (400, clamp 1.25 to 1.65rem, 1.35): the hero positioning line (max 34ch) and the About lead paragraph.
- **Title** (700, 1.3rem, 1.3, -0.01em): work row titles.
- **Body** (400, 1.0625rem, 1.6): running copy, capped at 62 to 64ch in ink-soft.
- **Label** (600, 0.8 to 0.85rem): band names, language switch, work band, marker band. The axis end labels ("Hardware", "Web") are the only uppercase text: 0.8rem, 600, 0.08em tracking.
- **Small** (400, 0.82 to 0.9rem): tags, citations, fact labels, marker subtitles.

### Named Rules
**The Thai Loosening Rule.** Under `lang="th"`, headings, the lead, and the contact email reset letter-spacing to 0, and the lead, section headings, About lead, and marker labels take line-height 1.5; the body moves from 1.6 to 1.75. Negative tracking is a Latin-only device.

**The One Family Rule.** Hierarchy comes from weight and size within the single stack. Do not introduce a second display face, a mono, or a system fallback as a display voice.

## Layout

A single centred column (max 1180px) with a fluid gutter (clamp 20 to 48px). Sections are separated by generous fluid top padding (clamp 72 to 128px), not by background changes.

Content inside sections is ruled grids rather than boxes. Section heads are a two-column grid (heading left, note right, bottom-aligned) closed by a 1px ink rule. Work rows are a three-column grid (180px band / flexible body / 220px meta) at 32px vertical padding, divided by hairlines. About reuses the 180px first column with a 260px facts column. The toolkit is four equal columns divided by vertical hairlines.

The header is sticky (64px), translucent ground (92% mix) with a 12px backdrop blur and a hairline bottom border. Anchored scroll offsets by 88px.

Responsive steps:
- **960px:** work rows collapse to band + meta on one line, body below; About stacks; toolkit goes to two columns.
- **760px:** nav and status separator hide; section heads stack; the spectrum turns vertical (see Components).
- **520px:** the brand name hides leaving the monogram; toolkit goes to one column with hairlines between groups; buttons tighten to 16px side padding.

## Elevation & Depth

The system is flat. There are no box-shadows anywhere. Depth is expressed by ruling (1px hairlines, a 1px ink rule under section heads), by one tonal inversion (the ink contact field and footer), and by the sticky header's translucent blur, which is the only layered surface.

### Named Rules
**The Ruled Not Raised Rule.** Group content with hairlines and alignment, never with cards, fills, or shadows. If something needs separation, it gets a rule.

## Shapes

Three forms only. Interactive controls (buttons, language switch and its segments, contact links) are full pills (999px). Markers, the band dot, and the "TK" monogram are circles. Everything else (rows, columns, the contact field, sections) is square-cornered and open, defined by rules rather than outlines. The range line itself has a 2px rounded cap; focus outlines carry a 2px radius.

## Components

### Buttons
Confident and quiet, ink-only.
- **Shape:** full pill (999px), 46px min height, 600 weight at 0.98rem, optional leading 1.1em stroke icon with a 10px gap.
- **Primary:** filled ink with ground text. Used once per view, for the resume download.
- **Quiet:** transparent with a 1px strong-hairline outline and ink text; hover darkens the outline to ink.
- **Hover / Active:** primary lifts to raised ink; any button presses down 1px on active. Transitions 0.2s.
- **Focus:** 2px range-blue outline, 3px offset (ground-coloured inside the ink contact field).

### Language Switch
- **Style:** a pill outline (1px strong hairline, 3px inset) holding two pill segments. The active segment is filled ink with ground text; the idle one is ink-soft text that darkens to ink on hover. The Thai segment carries `lang="th"` so it renders in Anuphan.

### Navigation
- **Style:** sticky translucent header with the circular ink "TK" monogram plus name at left, four text links in ink-soft (0.95rem) that darken to ink on hover, and the language switch at right. Below 760px the links hide and the header keeps brand plus language switch.

### Work Row
- **Style:** a ruled grid row. Left: the band label in its range colour, preceded by a 9px dot in the same colour. Centre: ink title (linked titles carry a small outbound stroke icon in ink-soft), ink-soft description, optional citation with the author's name in ink. Right: tags as a plain ink-soft list, or a "kind" label in ink.
- **Lit state:** a 2px rule in the row's band colour draws in from the left along the top edge (0.5s) and the title turns the band colour. Triggered by the paired marker's hover/focus, by hover/focus within the row, or by the row being the URL target.

### Contact Field
- **Style:** solid ink section with a 4px range stripe across its top edge, a display-scale heading, on-ink-mist note, a large underlined email (underline brightens on hover), and pill links outlined in on-ink hairline that brighten to ground on hover. The footer continues the ink field below a darker hairline.

### Range Spectrum (signature)
The page's signature and the only place colour is shown in full.
- **Desktop:** four band labels over proportional columns (22/30/22/26) divided by hairlines, a 200px track with a 4px gradient line through its centre, and circular markers placed by percentage position. Each marker is a 14px ground disc with a 3px ring in its band colour and a short strong-hairline leader to its label (bold title over an ink-soft subtitle). Labels alternate above and below the line so neighbours never collide; the last marker's label right-aligns. Uppercase "Hardware" and "Web" sit at the two ends over a hairline.
- **Below 760px:** the range turns vertical. The band header hides, the line runs top to bottom on the left (same stops, 180deg), markers stack in a 18px-gap list beside it, each marker shows its band name in its band colour, and "Hardware" and "Web" cap the top and bottom.
- **Lit state:** the marker ring fills with its colour and scales to 1.35x, and its title turns the band colour; its work row lights at the same time (see Work Row).
- **Motion:** on load the line draws from its start (scaleX, or scaleY when vertical) over 1.1s, then markers fade and rise 6px into place over 0.7s, staggered by position. This is the only entrance motion in the system. Easing is a long out-curve (cubic-bezier(0.16, 1, 0.3, 1)). Under reduced motion, all animation and transition is disabled and the spectrum appears static.

## Do's and Don'ts

### Do:
- **Do** keep colour bound to the range: a range stop only on something placed at that point on hardware-to-web, and the full four-stop gradient (0/38/62/100) only when drawing the whole range.
- **Do** separate content with 1px hairlines (rule) and close section heads with a 1px ink rule.
- **Do** make every interactive control a full pill (999px) and every marker a circle.
- **Do** reset negative tracking to 0 and loosen leading for Thai (1.5 on display-ish text, 1.75 body).
- **Do** keep any new motion to state transitions (0.2 to 0.5s on the system ease) and honour reduced motion by disabling it.
- **Do** keep icons as inline 1.8-stroke SVG at 1.1em in currentColor.

### Don't:
- **Don't** use cards, filled panels, or box-shadows on the light ground.
- **Don't** use range hues as decorative accents, status colours, or headings for things not on the range (toolkit headings stay ink).
- **Don't** add a coloured status dot or badge to availability text.
- **Don't** introduce a second hue family or a tinted background other than the ink contact field.
- **Don't** add entrance animation beyond the spectrum's single load moment.
