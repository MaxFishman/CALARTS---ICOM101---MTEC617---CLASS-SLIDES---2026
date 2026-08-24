# Week 03 Teacher Guide — Introduction to CSS

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 03 — Introduction to CSS**
> _Teacher Guide_

## At a glance

This is a 20-slide lecture introducing CSS (Cascading Style Sheets), the language we use to style HTML structure. Students learn the anatomy of a ruleset, where CSS can live, how to link an external stylesheet, the box model, sizing and spacing, borders and border-radius, overflow, the universal-selector reset, and typography (font-family stacks, weight/style/case, text layout, and web fonts). The week closes with a homework slide asking students to style a project. Prerequisite: Weeks 01–02.

## Learning objectives

By the end of this week, students should be able to:

- Explain what CSS is and what it's for: if it's about how a page looks, CSS is the tool.
- Read a ruleset and name its parts (selector, declaration block, declaration, property, value).
- Describe the three places CSS can go and identify external stylesheets as best practice.
- Link an external stylesheet with `<link>` in the `<head>`.
- Explain the box model and use padding, margin, and borders.
- Size and center boxes, and manage overflow.
- Apply a CSS reset with the universal selector.
- Style type with font stacks, weight/style/case, and text-layout properties.
- Load a web font from Google Fonts.

## Key terms

- **Ruleset:** A complete CSS rule, e.g. `h1 { color: blue; }`.
- **Selector:** Targets the element (every `<h1>`).
- **Declaration block:** Everything inside `{ }`.
- **Declaration:** One property: value pair (`color: blue;`). End with a semicolon.
- **Property:** The characteristic (`color`).
- **Value:** What you set it to (`blue`).
- **Inline CSS:** `<p style="color:red;">Hi</p>` — quick, rarely used.
- **Internal CSS:** `<style> p { color:red; } </style>` inside `<head>` — better, still not best.
- **External CSS:** A separate `.css` file — HTML stays clean, CSS maintainable. Best practice.
- **`<link>` — href & rel:** `href` = path to the CSS file; `rel` = the relationship, always "stylesheet". `<link>` lives in `<head>` and is self-closing. Without it, no styles apply.
- **Box model:** Every element lives in a box — margin (space outside) → border (the frame) → padding (space inside) → content (the text or image).
- **px (pixels):** An exact size, the same on every device.
- **border-radius:** Rounds corners; equal width & height + 50% makes a perfect circle.
- **padding:** Space inside — the mat between a picture and its frame. Use padding-top/-right/-bottom/-left for one side.
- **margin `0 auto`:** Centers a block horizontally — 0 sets top/bottom, auto splits leftover space evenly. Only works with a set width.
- **Margin collapse:** Vertical margins collapse — the browser keeps the LARGER of two stacked vertical margins. Padding never collapses.
- **overflow (visible/hidden/scroll):** visible → spills outside (default); hidden → clipped/hidden; scroll → adds a scrollbar.
- **Universal selector `*`:** Targets every element; often used for the reset.
- **font-family / font stack:** Lists fallbacks; the browser tries each until one is available, ending with a generic keyword (serif/sans-serif). Wrap multi-word names in quotes.
- **font-weight / font-style / text-transform:** `font-weight` uses keywords (normal/bold) or 100–900 (400 normal, 700 bold); `font-style: italic;`; `text-transform: uppercase;`.
- **letter-spacing / word-spacing / line-height / text-align:** Text-layout properties. Prefer unitless line-height (scales with font size); use em for spacing.
- **Web fonts:** Web-safe fonts are reliable but limited; web fonts (Google Fonts, Adobe Fonts) let you use almost any typeface.

## Lesson flow

**Slide 1 — Title.** "Introduction to CSS."

**Slide 2 — What is CSS.** "HTML builds it. CSS makes it beautiful." CSS = Cascading Style Sheets, the language we use to style HTML structure. Colors, fonts, sizes, images, spacing, positioning — if it's about how a page looks, CSS is the tool.

**Slide 3 — Ruleset.**
```css
h1 { color: blue; }
```
selector targets the element (every `<h1>`); declaration block is everything inside `{ }`; declaration is one property: value pair (`color: blue;`); property is the characteristic (`color`); value is what you set it to (`blue`). End with a semicolon.

**Slide 4 — Where CSS goes.**
```html
<p style="color:red;">Hi</p>
<style> p { color:red; } </style>
```
1 Inline (quick, rarely used). 2 Internal, inside `<head>` (better, still not best). 3 External — a separate `.css` file: HTML stays clean, CSS maintainable (✓ best practice).

**Slide 5 — Linking.** Inside `<head>`:
```html
<link href="styles/style.css" rel="stylesheet">
<link href="./style.css" rel="stylesheet">
```
href = path to the CSS file; rel = the relationship, always "stylesheet". `<link>` lives in `<head>` and is self-closing. Without it, no styles apply.

**Slide 6 — Box model.** Every element lives in a box: margin (space outside) → border (the frame) → padding (space inside) → content (the text or image).

**Slide 7 — Height & width.**
```css
p { height: 80px; width: 240px; }
```
`px` = pixels, an exact size the same on every device. A pixel-width box that fills a laptop will overflow a phone.

**Slide 8 — Borders.**
```css
p { border: 3px solid coral; }
```
Three values: width (px or thin/medium/thick), style (solid, dotted, none…), color (140 named colors or a code).

**Slide 9 — Border-radius.**
```css
.card { border: 3px solid blue; border-radius: 12px; }
.dot { border-radius: 50%; }
```
Equal width & height + 50% makes a perfect circle.

**Slide 10 — Padding.**
```css
.box { border: 3px solid coral; padding: 16px; }
padding-bottom: 16px;
```
Padding is the mat between a picture and its frame. Use padding-top/-right/-bottom/-left for one side.

**Slide 11 — Margin & centering.**
```css
p { margin: 20px; }
.headline { width: 400px; margin: 0 auto; }
```
`margin: 0 auto` centers a block horizontally — 0 sets top/bottom, auto splits leftover space evenly. Only works with a set width.

**Slide 12 — Margin collapse.** Horizontal margins add (two 20px = 40px apart). Vertical margins collapse — stacked 10px & 30px sit 30px apart (browser keeps the LARGER). // remember — padding never collapses.

**Slide 13 — Overflow.**
```css
.box { overflow: scroll; }
```
visible → spills outside (default); hidden → clipped/hidden; scroll → adds a scrollbar.

**Slide 14 — Reset.**
```css
* { margin: 0; padding: 0; }
```
Every browser ships a hidden user-agent stylesheet (defaults). `*` is the universal selector — targets every element. Often the first rule in an external stylesheet.

**Slide 15 — Font-family.**
```css
h1 { font-family: Georgia, 'Times New Roman', serif; }
```
A font stack lists fallbacks; the browser tries each until one is available, ending with a generic keyword (serif/sans-serif). Wrap multi-word names in quotes. Serif has little feet; sans-serif is clean/no feet.

**Slide 16 — Weight/style/case.**
```css
font-weight: 700; /* or bold */
font-style: italic;
text-transform: uppercase;
```
font-weight: keywords (normal/bold) or 100–900 (400 normal, 700 bold).

**Slide 17 — Text layout.**
```css
letter-spacing: 2px; word-spacing: 0.3em; line-height: 1.4; text-align: center;
```
Prefer unitless line-height (scales with font size); use em for spacing.

**Slide 18 — Web fonts.** Link a font (Google Fonts) in `<head>`:
```html
<link href="…fonts.googleapis.com/…Roboto" rel="stylesheet">
```
```css
h1 { font-family: 'Roboto', sans-serif; }
```
Web-safe fonts are reliable but limited; web fonts (Google Fonts, Adobe Fonts) let you use almost any typeface. Extra-credit territory for the homework.

**Slide 19 — Recap.** Chips: ruleset, selector, inline/internal, external + `<link>`, box model, margin, border, padding, border-radius, overflow, `*` reset, font-family, font-weight/style, line-height/align, web fonts.

**Slide 20 — Homework.** "Style your project" (see "Homework to assign" below).

## Watch out for

- External stylesheets are best practice — keep steering students there over inline and internal.
- `<link>` is self-closing and lives in the `<head>`. Without it, no styles apply.
- `margin: 0 auto` only works with a set width.
- Vertical margins collapse to the LARGER value; padding never collapses.
- Prefer unitless line-height (it scales with font size); use em for spacing.

## Discussion prompts

- **Slide 12 // remember:** "padding never collapses." Ask students to contrast this with vertical margin collapse.
- **Slide 19 // the big idea:** "external stylesheets are best practice: keep HTML for structure, CSS for style." Ask why separating structure from style makes a project easier to maintain.

## Homework to assign

**Style your project.** Fork last week's assignment (or start a fresh project). Add CSS to style your HTML:

- Use the box model: padding, margin, or a border.
- Change an element's color or background-color.
- Change an element's font from the default.
- Use at least one class attribute to style some HTML selectively.
- If you didn't last week — add an `<img>` and an `<a>` tag.
- **[extra credit]** Load a font from Google Fonts.

## Looking ahead

Up next: selectors & the cascade.
