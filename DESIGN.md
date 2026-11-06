---
name: "Cafeteria 15L"
description: "A Downtown comfort-food editorial homepage, with the existing inner-page system preserved."
colors:
  paper: "#f4f0e7"
  ink: "#292a22"
  muted: "#626157"
  accent: "#a23f27"
  on-accent: "#fff7e8"
  line: "#292a2233"
  panel: "#e9e5d9"
  home-paper: "#f4f0e7"
  home-ink: "#292a22"
  home-muted: "#645e54"
  home-accent: "#9d402b"
  home-on-accent: "#fff7e8"
  home-line: "#292a2233"
  home-panel: "#e8e1d4"
  home-photo-ink: "#fff8e9"
  home-photo-line: "#fff8e987"
  home-room-surface: "#e9e3d6"
typography:
  display:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(85px,10vw,152px)"
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: "-.04em"
  display-mobile:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(64px,18vw,105px)"
    fontWeight: 400
    lineHeight: 0.94
    letterSpacing: "-.04em"
  headline:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(38px,4.8vw,70px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.025em"
  title:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(27px,3vw,42px)"
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: "-.025em"
  body:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.65
  navigation:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "14px"
    fontWeight: 400
  button:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.2
  home-headline:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(44px,5.8vw,88px)"
    fontWeight: 400
    lineHeight: 1.03
    letterSpacing: "-.035em"
  home-story:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(25px,3vw,43px)"
    fontWeight: 400
    lineHeight: 1.27
    letterSpacing: "-.025em"
  home-menu-title:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(25px,2.3vw,34px)"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "-.025em"
  inner-page-title:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(56px,7.7vw,112px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.025em"
  home-eyebrow:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: ".11em"
rounded:
  control: "2px"
  square: "0"
spacing:
  gutter: "clamp(22px,4.3vw,76px)"
  section: "clamp(64px,8vw,128px)"
  gutter-mobile: "22px"
  section-mobile: "65px"
  gutter-narrow: "18px"
  actions: "12px"
  home-gutter: "clamp(22px,4.3vw,76px)"
  home-section: "clamp(76px,9vw,144px)"
  home-section-mobile: "72px"
  home-gallery-gap: "24px"
components:
  inner-button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.on-accent}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 25px"
  inner-button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 25px"
  inner-gallery-control:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    padding: "12px 17px"
  inner-event-faq:
    textColor: "{colors.ink}"
  home-button-primary:
    backgroundColor: "{colors.home-accent}"
    textColor: "{colors.home-on-accent}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 25px"
  home-button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.home-photo-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.control}"
    padding: "15px 25px"
  home-navigation:
    textColor: "{colors.home-ink}"
  home-menu-copy:
    textColor: "{colors.home-ink}"
  home-map-panel:
    backgroundColor: "{colors.home-panel}"
    textColor: "{colors.home-ink}"
    padding: "35px"
  home-weekly-item:
    textColor: "{colors.home-ink}"
---

# Design System: Cafeteria 15L

## Overview

**Creative North Star: "A Downtown comfort-food editorial"**

A Downtown comfort-food editorial. A full-bleed marquee-room photograph carries giant low-set serif type. The ruled edition strip remains above it. Desktop height is calc(100svh - 126px), bounded by 790px and 980px; mobile uses a 770px minimum and starts the copy near the top. The photograph shifts its crop to 65% 50% on mobile.

The inner pages retain their earlier ivory, brick and warm-stone palette. The homepage adjusts brick, muted text and panel values while keeping the same font pairing.

**Key Characteristics:**

- A Downtown comfort-food editorial.
- Eight complete homepage content sections grounded in real menu and venue evidence.
- Text-only actions, real photographs and restrained motion with reduced-motion support.

The homepage loads `assets/styles.css` and `assets/app.js`, then `assets/pitch.css` and `assets/pitch.js`. Inner routes keep the original stylesheet and script. Current homepage direction and facts are in `data/pitch-direction.md` and `data/revision-facts.json`; screenshots are in `preview/`. This is a code-led record, with no approved comp, generated seed, detector result or certification claimed. Read `QA.md` for the recorded verification scope.

Research links retained from `data/design-research.json`: [Tripletta Pizza](https://www.awwwards.com/sites/tripletta-pizza) (Awwwards Site of the Day, 2025-04-04); [Cantina del Sol](https://www.cssdesignawards.com/sites/cantina-del-sol/46113/) (CSS Design Awards Website of the Day, 2024-08-22); [Luckyfolks](https://www.cssdesignawards.com/sites/luckyfolks/38327/) (CSS Design Awards Website of the Day, 2021-01-08). These are research references, not awards for this concept.

## Colors

Unprefixed colors retain the inner-page palette. `home-*` colors are the effective homepage values after the body override; inherited line and on-accent values are preserved exactly. The frontmatter is normative.

### Primary

`accent` / `on-accent` belong to inner-page actions. `home-accent` / `home-on-accent` belong to homepage actions, with the scoped reversals below.

### Neutral

`home-paper`: ivory; `home-ink`: olive charcoal; `home-muted`: warm gray; `home-accent`: marquee brick; `home-on-accent`: warm cream; `home-line`: translucent olive charcoal; `home-panel`: warm stone. The opening uses `home-photo-ink` on the photograph and `home-photo-line` for secondary-action borders; the room section uses `home-room-surface`.

**The Route Scope Rule.** Homepage tokens apply only with the pitch-home body class. Preserve the existing inner-page tokens for routes that do not load pitch.css.

Sidecar OKLCH ramps are derived swatch previews, not additional implemented palette tokens.

## Typography

Display type remains DM Serif Display, Georgia, serif; body and control type remains DM Sans. The local WOFF2 faces use font-display:swap. `display` and `display-mobile` now describe the current homepage H1; `home-headline`, `home-story` and `home-menu-title` describe its other display roles. Unprefixed `headline`/`title` and `inner-page-title` retain the inner-page hierarchy.

The homepage headline is “Meatloaf. Marquee. 15th & L.”. Its story lead is separate from supporting copy: the latter is 15px/1.7 with a 47ch maximum, then 14px on mobile. Homepage section headings generally become 43px at 650px and below and 38px at 360px and below; contextual event and weekly headings retain their scoped sizes. Menu-entry titles become 27px/1.12 on mobile. Inner-page H1s become 54px at 650px and below and 44px at 360px and below, with long-word wrapping.

## Layout

The homepage contract has eight content sections: hero, short story, six real menu picks, room gallery, private events, weekly programming, visit/parking/map, and footer with gift cards, MAC Rewards and sister venues. Cafeteria retains the edition strip. A 1fr / 1fr menu spread combines a tall photograph, a smaller offset food image and six ruled entries. Mobile hides the small food image and stacks the main photograph above the list.

The outer shell remains capped at 1800px. Homepage sections use `home-gutter` and `home-section`; at 650px and below they use a 22px gutter and the 72px section token, with an 18px gutter at 360px and below. The header is 88px tall, then 78px at 900px and below and 76px at 650px and below. Navigation becomes a disclosure at 900px and below. Galleries, event blocks, visits and menu spreads become one-column at 650px and below. The mobile second gallery image remains 430px high while the other two are 350px.

Inner pages retain their `gutter`/`section` spacing, 65px mobile section rhythm, and existing responsive menu, event, location and gallery layouts in `assets/styles.css`.

## Elevation & Depth

The interface is flat: photography, solid tonal sections, photographic legibility overlays and ruled borders provide depth. No box shadows are defined. The gallery dialog uses its existing dark translucent backdrop.

**The Flat Surface Rule.** Use tonal surfaces, rules and real photography for depth. Do not add box shadows.

## Shapes

Current homepage photographs and panels have square corners. Buttons and the navigation toggle retain the 2px control radius. Inner pages keep square image and panel frames, 2px action corners, bordered native dialogs and simple ruled information sections. The former homepage hero composition is no longer the current homepage contract.

## Components

### Actions and navigation

Homepage actions retain the primary/secondary token variants, 1px borders and 50px minimum height. At 650px and below they use 13px type, 14px 18px padding and a 48px minimum; at 360px and below they use 12px type and 13px 15px padding. Source-specific photographic and header reversals are captured in the color scope above. Inner-page buttons retain their earlier 14px labels and 50px minimum, becoming 49px on mobile.

Keep text-only labels and the visible 3px focus outline with a 5px offset. The menu closes on Escape, link selection, outside click and desktop resize. Escape restores focus to its toggle. Underlined navigation hover/current states and official transaction destinations remain intact.

### Menu, rooms and events

Each homepage has six actual selections linked to current official menus. The final menu-entry layout is one column with no numbered rail. Three room-gallery controls open the existing native dialog; preserve Previous/Next, arrow keys, Escape, backdrop close and opener focus restoration. Event panels pair a real photograph with source-backed details, capacity text and inquiry actions. Do not fabricate a local booking form.

### Weekly strip, visit and footer

Keep weekly restrictions adjacent to their schedule. Visit cards show current branch hours, parking guidance and the appropriate map address. Show map creates the titled Google Maps iframe only after activation, then focuses it; there is no initial map embed. Footer actions retain gift-card destinations, MAC Rewards and the sibling-venue links without inventing service terms.

### Motion

The opening photograph uses requestAnimationFrame parallax clamped to ±14px, with a 110%-height image starting 5% above its frame. There are no generic section-rise or entrance animations. Room photographs scale to 1.04 over 0.5s on hover. Menu-entry padding/color transitions last 0.25s. Buttons retain their 0.2s state transition. Smooth scrolling remains enabled. Reduced-motion disables animation and transitions, resets parallax, and switches scrolling to auto.

## Do's and Don'ts

### Do:

- Do keep the homepage and inner-page palettes scoped to their own routes.
- Do preserve the eight-section homepage sequence and all six real menu selections.
- Do keep location, photo, programming and service-link claims tied to data/revision-facts.json.
- Do retain visible focus, text-only 2px controls, keyboard gallery behavior and click-to-load maps.

### Don't:

- Don't reuse another venue's opening, typography treatment or signature composition.
- Don't add a hero overline or repeated section-rise entrances; keep the existing edition strip.
- Don't invent reviews, awards, quotes, founder details, menu items or parking guarantees.
- Don't use generic hospitality slogans, decorative arrows, highlighted words, tilted labels, theme switches or em dashes in homepage copy.
