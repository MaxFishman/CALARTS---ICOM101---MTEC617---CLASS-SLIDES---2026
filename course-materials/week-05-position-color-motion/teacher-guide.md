# Week 05 Teacher Guide — Position, Color & Motion

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 05 — Position, Color & Motion**
> _Teacher Guide_

## At a glance

- **Course:** Intro to Web Development — ICOM101 / MTEC617, CalArts, Spring 2026 (9-week course)
- **Instructor:** Max Fishman — mfishman@calarts.edu, (626) 463-3100
- **Week:** 05 — Position, Color & Motion
- **Format:** 19-slide lecture, in three acts — **place it, paint it, move it.**
- **Prerequisite:** Weeks 01–04
- **Ends with:** a homework checklist on slide 19 ("Make it move")

The lecture is organized as three acts: **01 Positioning** (relative/fixed/sticky/z-index), **02 Color & Backgrounds** (color/opacity/background-image), and **03 Transitions** (duration/timing/delay).

## Learning objectives

By the end of the week, students should be able to:

- Explain that every element is `position: static` by default and that offsets do nothing until you change that.
- Use `relative`, `fixed`, and `sticky` positioning and the offset properties `top`, `bottom`, `left`, `right`.
- Layer overlapping positioned boxes with `z-index`.
- Set foreground and background color, adjust `opacity`, and apply a `background-image` or a gradient.
- Style a `:hover` state change.
- Write a `transition` that controls property, duration, timing, and delay — including the shorthand.

## Key terms

- **`position: static`** — the default; every element starts in normal flow.
- **`position: relative`** — positions an element relative to its own default spot; the space it used to occupy is left behind.
- **`position: fixed`** — locks an element to a spot on the screen; it ignores scrolling. Great for headers, nav bars, "back to top" buttons.
- **`position: sticky`** — scrolls normally until it hits your offset, then sticks there until its parent scrolls past.
- **Offset properties** — `top` (moves down from the top), `bottom` (moves up from the bottom), `left` (moves away from the left), `right` (moves away from the right). Values in px, em, or %.
- **`z-index`** — when positioned boxes overlap, sets their depth; a higher number sits in front.
- **`color` vs `background-color`** — `color` sets the foreground (usually the text); `background-color` paints the box behind it.
- **`opacity`** — runs from 0 (fully invisible) to 1 (fully solid); 0.5 is half-transparent, perfect for overlays.
- **`background-image` / `url(…)`** — the value is a `url(…)`: a relative path to a file in your project or a full web address.
- **Linear vs radial gradient** — a gradient is a smooth blend between colors, no image file needed. `linear` runs in a direction; `radial` spreads out from a point.
- **`:hover` state change** — applies styles only while the pointer is over an element.
- **`transition`** — controls how a state change happens over time; instead of snapping, it eases. Controls four things: **property** (which CSS property animates), **duration** (how long it takes), **timing** (how it accelerates), **delay** (how long to wait before it starts).
- **Timing functions** — `ease` (slow → fast → slow, the default), `linear` (constant speed), `ease-in` (starts slow, accelerates, stops abruptly), `ease-out` (starts abruptly, slows to a gentle stop).
- **Transition shorthand & `all`** — `transition: color 1.5s linear 0.5s;` (order: property duration timing delay); `transition-property: all;` animates every property that changes.

## Lesson flow

**S1 — Title.** "Position, Color & Motion."

**S2 — Overview.** "Place it, paint it, move it." Three acts: 01 Positioning (relative/fixed/sticky/z-index); 02 Color & Backgrounds (color/opacity/background-image); 03 Transitions (duration/timing/delay).

**S3 — The position property.** By default every element is `position: static` (normal flow). Change position to unlock four offset properties: `top` → moves down from the top; `bottom` → moves up from the bottom; `left` → moves away from the left; `right` → moves away from the right. Values in px, em, or % — but offsets do NOTHING while position is still static.

**S4 — Relative.**
```css
.green-box {
  background-color: green;
  position: relative;
  top: 50px;
  left: 120px;
}
```
`relative` positions an element relative to its own default spot (50px down, 120px right). The space it used to occupy is left behind.

**S5 — Fixed.**
```css
.title {
  position: fixed;
  top: 0px;
  left: 0px;
}
```
`fixed` locks an element to a spot on the screen — it ignores scrolling. Great for headers, nav bars, "back to top" buttons.

**S6 — Sticky.**
```css
.box-bottom {
  background-color: darkgreen;
  position: sticky;
  top: 240px;
}
```
`sticky` scrolls normally until it hits your offset (`top: 240px`), then sticks there until its parent scrolls past.

**S7 — z-index.**
```css
.blue-box { position: relative; z-index: 2; }
.green-box { position: relative; z-index: 1; }
```
When positioned boxes overlap, `z-index` sets their depth — a higher number sits in front.

**S8 — Color.**
```css
h1 {
  color: red;
  background-color: gold;
}
```
`color` sets the foreground (usually the text); `background-color` paints the box behind it.

**S9 — Opacity.**
```css
.overlay { opacity: 0.5; }
```
Opacity runs from 0 (fully invisible) to 1 (fully solid). 0.5 is half-transparent — perfect for overlays.

**S10 — Background-image.**
```css
.main-banner { background-image: url('images/mountains.jpg'); }
```
or `url('https://…/photo.jpg')`. The value is a `url(…)` — a relative path to a file in your project or a full web address.

**S11 — Gradients.**
```css
background: linear-gradient(to right, red, blue);
background: radial-gradient(circle, red, blue);
```
A gradient is a smooth blend between colors — no image file needed. `linear` runs in a direction; `radial` spreads out from a point.

**S12 — Hover.**
```css
a {
  color: purple;
  text-decoration: underline dotted;
}
a:hover {
  color: goldenrod;
  text-decoration: underline;
}
```
`:hover` applies styles only while the pointer is over an element — a state change. Right now the change snaps instantly.

**S13 — Transitions.** A transition controls how a state change happens over time — instead of snapping, it eases. Control four things: **property** → which CSS property animates; **duration** → how long it takes; **timing** → how it accelerates; **delay** → how long to wait before it starts. `// hover the buttons on the next slides — the demos are live.`

**S14 — Duration.**
```css
.btn {
  transition-property: all;
  transition-duration: 0.4s;
}
```
A transition needs at least a property and a duration. Time in seconds or milliseconds — `1s`, `0.4s`, `400ms`.

**S15 — Timing.** `ease` → slow → fast → slow (the default); `linear` → constant speed; `ease-in` → starts slow, accelerates, stops abruptly; `ease-out` → starts abruptly, slows to a gentle stop. All travel the same distance in the same time — only the pacing differs.

**S16 — Delay.**
```css
transition-property: width;
transition-duration: 750ms;
transition-delay: 250ms;
```
A width change waits 250ms, then animates over 750ms. Default delay is `0s`.

**S17 — Shorthand.**
```css
transition: color 1.5s linear 0.5s;
```
(order: property duration timing delay); chain with commas:
```css
transition: color 1s linear, font-size 750ms ease-in 100ms;
```
and `transition: all 1.5s linear 0.5s;`. Gotcha: to set a delay you must also set a duration — the browser reads the first time value as the duration.

**S18 — Recap chips:** position:relative, fixed, sticky, top/bottom/left/right, z-index, color, background-color, opacity, background-image, gradients, :hover, transition, duration/timing/delay, all.

**S19 — Homework "Make it move":** Add a fixed or sticky header to your project. Give an element a background-color, background-image, or gradient. Style a link's :hover state. Add a transition so that hover change eases in smoothly. Curious? Overlap two boxes and control them with z-index. Closing: small motion, big polish.

## Discussion prompts

- **On transitions (from slide 13):** `// hover the buttons on the next slides — the demos are live.` Have students predict how a hover will feel before you show the live demo, then compare `ease`, `linear`, `ease-in`, and `ease-out` on the same button.
- **The big idea (from slide 18):** `// the big idea — positioning places things, color gives them life, and transitions make change feel smooth instead of sudden.` Ask students to point to one place in their own project where each of the three acts is doing its job.

## Watch out for

- **Offsets do NOTHING while position is still static.** If a student sets `top`/`bottom`/`left`/`right` and nothing moves, the first thing to check is whether they changed `position` away from the default `static`.
- **To set a transition delay you must also set a duration.** In the shorthand, the browser reads the *first* time value as the duration. So `transition: color 0.5s;` is a half-second duration, not a delay — students who want a delay must supply both time values (e.g. `transition: color 1.5s linear 0.5s;`).

## Homework to assign

Assign the slide-19 checklist ("Make it move"), expanded in `assignment.md`:

1. Add a fixed or sticky header to the project.
2. Give an element a `background-color`, `background-image`, or gradient.
3. Style a link's `:hover` state.
4. Add a transition so the hover change eases in smoothly.
5. **Optional:** overlap two boxes and control them with `z-index`.

## Looking ahead

Keep steering students toward the closing line: **small motion, big polish.** A little bit of positioning, color, and eased motion goes a long way — the goal is change that feels smooth instead of sudden, not animation for its own sake.
