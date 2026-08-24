# Week 05 Homework — Position, Color & Motion

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 05 — Position, Color & Motion**
> _Assignment_

## Overview

This week is all about three moves: **place it, paint it, move it.** You'll take the project you've been building and give it a header that stays put, add some color or a background, make a link react when the pointer is over it, and finally make that reaction ease in smoothly instead of snapping. The homework is called **"Make it move."**

## What you'll practice

- **Positioning** — using `position: fixed` or `position: sticky` so an element stays on screen or sticks as you scroll.
- **Color & backgrounds** — setting a `background-color`, a `background-image`, or a gradient.
- **State changes** — styling a link's `:hover` state.
- **Transitions** — adding a `transition` so a hover change eases in smoothly instead of snapping.
- **(Optional) z-index** — overlapping two boxes and controlling which one sits in front.

## The assignment

Work on the project you already have. Complete these four required steps, plus the optional challenge if you're curious.

1. **Add a fixed or sticky header to your project.**
   Use `position: fixed` (locks to a spot on the screen and ignores scrolling) or `position: sticky` (scrolls normally until it hits your offset, then sticks). Pick whichever fits your layout.

2. **Give an element a `background-color`, `background-image`, or gradient.**
   Any one of the three is fine:
   - a solid `background-color`,
   - a `background-image` using `url(…)` — a relative path to a file in your project or a full web address, or
   - a `linear-gradient` or `radial-gradient` (a smooth blend between colors, no image file needed).

3. **Style a link's `:hover` state.**
   Give a link a normal look, then use `:hover` to change something (for example its `color`) only while the pointer is over it.

4. **Add a transition so that hover change eases in smoothly.**
   Add a `transition` so the state change happens over time instead of snapping instantly. Remember a transition needs at least a **property** and a **duration**.

**Curious? (optional challenge):** Overlap two boxes and control them with `z-index` — the higher number sits in front.

## Submission

- Submit your project files (HTML and CSS).
- Make sure your header stays on screen when you scroll, and that your hovered link eases into its new state rather than snapping.
- Questions? Email Max Fishman at mfishman@calarts.edu or call (626) 463-3100.

## How it's graded

This is a light checklist — each required piece is either present and working or not.

| Requirement | Done? |
| --- | --- |
| Fixed or sticky header added | ✔ / — |
| An element has a background-color, background-image, or gradient | ✔ / — |
| A link's `:hover` state is styled | ✔ / — |
| A transition makes the hover change ease in smoothly | ✔ / — |
| **Optional:** two boxes overlapped and layered with `z-index` | bonus |

_Closing thought from lecture: small motion, big polish._
