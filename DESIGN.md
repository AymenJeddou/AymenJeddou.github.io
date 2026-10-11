---
name: Aymen Jeddou, portfolio
description: The Verdict Sheet: indigo night and saffron, a candidate card, every claim with its proof line.
colors:
  navy: "#17193b"
  navy-2: "#3f47b0"
  navy-line: "#3b3f72"
  on-navy: "#eef0ff"
  on-navy-2: "#b9bee8"
  coral: "#f4b740"
  coral-ink: "#2a1a00"
  coral-deep: "#94570a"
  go: "#17734b"
  go-bg: "#e4f4ec"
  ground: "#f3f4f8"
  surface: "#ffffff"
  ink: "#161827"
  ink-2: "#4a4d63"
  line: "#dee0ea"
typography:
  display:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(3.6rem, 8.5vw, 6rem)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(2rem, 4vw, 3rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.6rem"
    fontWeight: 700
    lineHeight: 1.05
  body:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Bricolage Grotesque, ui-sans-serif, system-ui, sans-serif"
    fontSize: "0.88rem"
    fontWeight: 400
    lineHeight: 1.5
rounded:
  frame: "14px"
  pill: "999px"
spacing:
  section: "112px"
  block: "56px"
  gutter: "32px"
components:
  button-primary:
    backgroundColor: "{colors.coral}"
    textColor: "{colors.coral-ink}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "48px"
  button-on-navy:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-navy}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "48px"
  pill-verdict:
    backgroundColor: "{colors.go}"
    textColor: "{colors.surface}"
    rounded: "{rounded.pill}"
  pill-status:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink-2}"
    rounded: "{rounded.pill}"
  frame:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.frame}"
---

## Overview

The portfolio borrows HiresHere's idea (a verdict plus the line that proves it) but has its own palette and no HiresHere logo: Aymen is the builder, not the brand. The green pill states the verdict ("Open for a PFE in data or AI, 2027") and every claim below carries the line that proves it. Navy owns the first viewport and the close; the light ground carries the work in between. Section headings are short and first person ("What I've built", "Where I've worked", "Get in touch"); all copy speaks as Aymen.

## Colors

Two inks do the work: indigo night (`navy` token, #17193b) as a full field for the hero and the close, saffron (`coral` token, #f4b740) as the only accent (the AJ monogram, the avatar ring, proof rules, the primary button, the full stop after the name). Token names are historical; the values are the palette. Verdict green (`go`) appears only where something is proven or live; it is never decoration. Light sections sit on `ground`, with `surface` for frames and the experience band. Text on navy uses `on-navy` and `on-navy-2`, never grey.

## Typography

One face, Bricolage Grotesque, self-hosted from `assets/fonts/bricolage.woff2` (variable weight, width and optical size). Display and headings use `opsz` 96 with tight tracking; body uses `opsz` 14. Weight steps: 800 name, 700 headings, 600 emphasis and buttons, 400 text.

## Layout

Single page, 1180px wrap with 32px gutters (20px on phones). Hero is a two-column grid: name, role, verdict pill and actions on the left, a candidate card on the right (HiresHere job-card style: the round portrait with a saffron ring overlapping its top edge, role, "Available" pill, skill tags, a quoted line with its source); no location or map; the HiresHere screenshot rises out of the hero's bottom edge. Projects alternate text and image columns (5:7 then 7:5) and stack under 960px. Sections are 112px apart (80px on phones), more space above a heading than below.

## Elevation & Depth

Flat fields with one depth device: project frames and the pin carry a soft, neutral drop shadow (`0 24px 48px -24px rgba(16,24,32,.28)`). No coloured glows.

## Shapes

Pills (999px) for buttons, verdicts and statuses; 14px corners for screenshot frames and the diagram panel, 18px for the candidate card. The emblem is the AJ monogram (10px-radius saffron tile); the HiresHere logo is not used.

## Components

- **Proof line**: a 2px coral left rule, a bold sentence naming the source and date, and a "How" disclosure (`<details>`) that expands the evidence.
- **Ruled scale**: before→after results on a 0 to 1 rule with ticks; open circle for before, green dot and green segment for the gain. Never a big-number tile.
- **Frame**: real screenshots in a white frame; a top bar shows the live URL when the project is live.
- **Status pills**: green "Live" for live sites, outlined "In progress", "Open PR", "Issue", "Discussion" for everything not finished. Statuses are honest.
- **Candidate card**: the hero's job card about Aymen; the README header (`AymenJeddou/assets/header.png`, rendered from `.impeccable/banner.html`) repeats it.
- **Motion**: hero lines rise in sequence, the card slides in and the avatar pops (ease-out expo); blocks reveal once on scroll; ruled scales move from before to after when seen; frames lift on hover; the verdict tick breathes slowly. All off under reduced motion, and content is visible without JavaScript.

## Do's and Don'ts

- Do show the real product: screenshots, live links, dated numbers.
- Do label third-party images with their credit (AgroScan's pest photo is CIRAD's).
- Don't add eyebrows or kickers above headings; dates and statuses go below the title.
- Don't set metrics as big-number tiles; inline bold figures or a ruled scale.
- Don't use verdict green for anything not proven, or saffron for a verdict.
- Don't reuse HiresHere's logo or exact palette.
- Don't list individual PRs or issues; open source is one line.
- Don't invent claims, testimonials or merged statuses.
