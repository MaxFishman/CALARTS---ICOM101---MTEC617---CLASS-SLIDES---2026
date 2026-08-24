# Week 04 Worksheet — Responsive Web Design

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 04 — Responsive Web Design**
> _Student Worksheet_

Responsive design means building one page that adapts its layout to whatever screen it lands on. Use this worksheet to practice media queries, breakpoints, and previewing your page across devices.

## Anatomy of a media query

Label the 4 parts of this media query:

```css
@media screen and (max-width: 600px) { body { font-size: 14px; } }
```

1. `@media` → ________________________________________
2. `screen` → ________________________________________
3. `(max-width: 600px)` → ________________________________________
4. `{ … }` (the `body { font-size: 14px; }` part) → ________________________________________

## Breakpoints

Match each device to its size range. Draw a line or write the letter.

| Device | | Size range |
| --- | --- | --- |
| 📱 Smartphone | ___ | A. min-width 1024px |
| 📋 Tablet | ___ | B. max-width 767px |
| 🖥 Desktop | ___ | C. 768px–1023px |

Reminder: these are common starting points, not hard rules. Set breakpoints where YOUR layout starts to break.

## Read & write the code

1. Write a media query that shrinks the `body` font size to `14px` when the viewport is 600px or smaller (≤600px).

```css
_________________________________________________________________
```

2. In Chrome DevTools, what is the keyboard shortcut to toggle the device toolbar?

`________________________________________`

## Short answer

1. In one sentence, what is responsive design?

________________________________________________________________

2. Name three ways to preview mobile.

________________________________________________________________

3. What does a CSS framework give you?

________________________________________________________________

4. Who makes Bootstrap, and who makes Material-UI?

- Bootstrap: ________________
- Material-UI: ________________

## Try it

Add one media query to your project — shrink text or stack columns on small screens. Then open Chrome DevTools (Cmd+Shift+M) and preview it across devices. Fix anything that overflows or breaks on phone width. Remember: keep testing on real screens.

## Answer key

**Anatomy of a media query**

1. `@media` → the keyword that begins a media query.
2. `screen` → the media type — almost always screen (vs print).
3. `(max-width: 600px)` → the condition — apply when viewport ≤600px; that width is a breakpoint.
4. `{ … }` → the styles used when the condition is true.

**Breakpoints**

- 📱 Smartphone → B. max-width 767px
- 📋 Tablet → C. 768px–1023px
- 🖥 Desktop → A. min-width 1024px

**Read & write the code**

1.

```css
@media screen and (max-width: 600px) { body { font-size: 14px; } }
```

2. Cmd/Ctrl + Shift + M

**Short answer**

1. Responsive design is building one page that adapts its layout to whatever screen it lands on.
2. Chrome DevTools; Xcode Simulator; Safari.
3. A pre-built library of styles and components (grids, buttons, forms, navigation) that make it faster to build responsive, consistent pages.
4. Bootstrap: by Twitter. Material-UI: by Google.
