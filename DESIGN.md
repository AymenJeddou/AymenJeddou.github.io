---
name: Aymen Jeddou, portfolio
description: The Verdict Sheet. A recruiter's question answered in HiresHere's verdict language, every claim with its proof line.
colors:
  navy: "#0b3a53"
  navy-2: "#155f80"
  navy-line: "#3a6c85"
  on-navy: "#f2f7fa"
  on-navy-2: "#b9d3e0"
  coral: "#ff7a59"
  coral-ink: "#2a0d05"
  coral-deep: "#c2410c"
  go: "#157a43"
  go-bg: "#e7f4ec"
  ground: "#f1f4f6"
  surface: "#ffffff"
  ink: "#14202b"
  ink-2: "#47515e"
  line: "#dde2e8"
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

The portfolio speaks HiresHere's language, because being the builder of HiresHere is the identity. A recruiter's question gets a verdict ("Open for a PFE in data or AI, 2027" in the green pill) and every claim below carries the line that proves it. Navy owns the first viewport and the close; the light ground carries the work in between. Section headings are the literal questions a recruiter asks.

## Colors

Two inks do the work: ocean navy (`navy`) as a full field for the hero and the close, coral (`coral`) as the only accent (the pin-and-check mark, proof rules, the primary button, the full stop after the name). Verdict green (`go`) appears only where something is proven or live; it is never decoration. Light sections sit on `ground`, with `surface` for frames and the experience band. Text on navy uses `on-navy` and `on-navy-2`, never grey.

## Typography

One face, Bricolage Grotesque, self-hosted from `assets/fonts/bricolage.woff2` (variable weight, width and optical size). Display and headings use `opsz` 96 with tight tracking; body uses `opsz` 14. Weight steps: 800 name, 700 headings, 600 emphasis and buttons, 400 text.

## Layout

Single page, 1180px wrap with 32px gutters (20px on phones). Hero is a two-column grid: name, role, verdict pill and actions on the left, a candidate card on the right (HiresHere job-card style: the portrait in the pin overlapping its top edge, role, "Available" pill, skill tags, a quoted line with its source); no location or map; the HiresHere screenshot rises out of the hero's bottom edge. Projects alternate text and image columns (5:7 then 7:5) and stack under 960px. Sections are 112px apart (80px on phones), more space above a heading than below.

## Elevation & Depth

Flat fields with one depth device: project frames and the pin carry a soft, neutral drop shadow (`0 24px 48px -24px rgba(16,24,32,.28)`). No coloured glows.

## Shapes

Pills (999px) for buttons, verdicts and statuses; 14px corners for screenshot frames and the diagram panel. The pin-and-check mark (from HiresHere's logo) is the only emblem.

## Components

- **Proof line**: a 2px coral left rule, a bold sentence naming the source and date, and a "How" disclosure (`<details>`) that expands the evidence.
- **Ruled scale**: before→after results on a 0 to 1 rule with ticks; open circle for before, green dot and green segment for the gain. Never a big-number tile.
- **Frame**: real screenshots in a white frame; a top bar shows the live URL when the project is live.
- **Status pills**: green "Live" for live sites, outlined "In progress", "Open PR", "Issue", "Discussion" for everything not finished. Statuses are honest.
- **Candidate card**: the hero's job card about Aymen; the README header (`AymenJeddou/assets/header.png`, rendered from `.impeccable/banner.html`) repeats it.
- **Pin drop**: the only entrance motion, once on load (0.9s, ease-out expo), disabled under reduced motion.

## Do's and Don'ts

- Do show the real product: screenshots, live links, dated numbers.
- Do label third-party images with their credit (AgroScan's pest photo is CIRAD's).
- Don't add eyebrows or kickers above headings; dates and statuses go below the title.
- Don't set metrics as big-number tiles; inline bold figures or a ruled scale.
- Don't use verdict green for anything not proven, or coral for a verdict.
- Don't invent claims, testimonials or merged statuses.
