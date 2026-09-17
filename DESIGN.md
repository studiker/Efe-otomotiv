---
version: alpha
name: Efe Oto Servis
description: Turkish automotive service concept with workshop photography and a WhatsApp request flow.
colors:
  primary: '#d52938'
  background: '#ffffff'
  navy: '#101d2b'
  ink: '#172532'
  muted: '#616b75'
  soft: '#f3f5f6'
  line: '#dde2e6'
  focus: '#126bcb'
typography:
  sans:
    fontFamily: 'Manrope, Arial, sans-serif'
  display:
    fontFamily: 'Barlow Condensed, Arial Narrow, Arial, sans-serif'
rounded:
  DEFAULT: '6px'
  sm: '4px'
  lg: '10px'
spacing:
  section-gap: '90px'
  page-max: '1240px'
components:
  button: {}
  card: {}
  dialog: {}
  field: {}
---

# Efe Oto Servis Design System

## Overview

### Creative North Star
An orderly independent workshop: graphite metal, clean signage, red equipment, and the mechanic's attention to the engine. Large condensed lettering recalls practical workshop signs.

### Product context and register
- Audience: drivers researching maintenance and repairs, primarily on mobile.
- Evidence: user's Turkish brief names Efe Oto Servis, previous work, Castrol/Shell and WhatsApp requests. Exact service location remains unprovided.
- Language: tr-TR. Native date/select popup language follows the visitor's operating system; formatted request dates use tr-TR.
- Register: marketing site with one lightweight local request preparation form; no customer database or admin workflow.
- Signature: full-width workshop photograph with disciplined oversized display type.
- Restraint: plain form controls, no invented ratings, years of experience or completed-job claims.
- Anti-reference: dealership stock inventory, racing-game UI, generic SaaS gradients.
- Runtime ownership: dist/style.css :root is canonical; this document mirrors semantic tokens. Components consume CSS variables. Navy → --navy, primary → --red, background → --paper, other color names map directly. Typography maps to --font-body and --font-display.

## Colors
White navigation and content surfaces contrast with the navy workshop hero. Red indicates primary actions and short category labels. Muted grey supports secondary descriptions. Focus uses the blue token. No theme toggle; forced-colors retains borders and platform colors.

## Typography
Barlow Condensed 700 for h1/h2; Manrope 400–800 for body and controls. Body uses 16px baseline, line-height 1.65. Small uppercase labels are secondary metadata. Controls have consistent labels and Turkish characters. Avoid fixed-height text containers.

## Layout
1240px maximum content width; desktop 48px side gutters, mobile 20px. Four service columns, three gallery columns; at 760px use two service columns and one gallery column; below 390px all are single-column. Full-width hero; two-column form becomes a stacked layout on mobile. Main document owns scrolling. Images have stable aspect ratios. Sticky mobile action includes safe-area spacing.

## Elevation & Depth
Flat bordered cards. Elevation only on modal and mobile action. Native dialogs provide modal layering and inert background. Sticky header stays above content and below dialogs.

## Shapes
6px primary controls and cards, 4px inputs, 10px modal. Circle buttons are compact secondary controls. No decorative shapes representing cars or mechanics.

## Components

### Foundational visual states
Shared buttons use hover darkening, visible blue focus, 1px pressed displacement, and disabled opacity. Fields reserve error space, associate labels, mark invalid state and focus the first invalid control. Status messages use role=status.

### Buttons and actions
Solid red is the main action. Navy is the copy action. Text actions use a small arrow. Labels describe preparation, not successful dispatch. All booking entry points share startBooking. Clipboard busy state disables duplicate click and keeps dimensions.

### Navigation and data display
Four anchor links. Mobile toggle exposes aria-expanded and supports Escape. Three gallery examples open the same detail dialog and can preselect the corresponding service. No invented public business contact details.

### Forms and overlays
Native select and native date are an intentional platform-owned choice, including popup geometry and operating-system locale. Form uses novalidate and local validation. Shared native dialog supplies focus containment, Escape close, background isolation and restoration. Values remain in form after closing the preview. No persistence or network submission occurs. WhatsApp requires configured real number; otherwise copy-only preview explains missing connection. Renders unknown contact values with textContent. Native calendar is not an availability calendar.

### Iconography
Simple stroked interface symbols for calendar, arrow, tools, diagnostics, brake, shield and chat. They accompany text. Official full-color Castrol/Shell SVGs are product-brand references, not partnership badges.

### Motion
30-second linear logo marquee, pause control and hover pause. Reduced-motion disables movement and smooth scrolling. Other transitions last 180–200ms. No entrance sequence blocks content.

### Content and data visualization
Turkish customer-facing copy, no charts. All gallery entries and detail views disclose representative concept imagery. The request is unconfirmed until service staff respond; no fake reservation success state.

## Do's and Don'ts
- Do preserve clear distinction between a prepared message, a message sent by the visitor and a confirmed appointment.
- Do replace representative gallery entries with actual consented work when supplied.
- Don't publish invented business facts or a random WhatsApp number.
- Don't imply authorized Castrol or Shell partnership.
