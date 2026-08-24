# Week 04 Teacher Guide — Responsive Web Design

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 04 — Responsive Web Design**
> _Teacher Guide_

## At a glance

Week 04 is a 14-slide lecture on responsive web design. Students learn to build one page that adapts its layout to whatever screen it lands on. The core tool is the media query. The lecture also covers breakpoints, three ways to preview mobile (Chrome DevTools, Xcode Simulator, Safari), why real devices still matter, and CSS frameworks (Bootstrap and Material-UI). It closes with a homework checklist on slide 14.

Prerequisite: Weeks 01–03.

Instructor: Max Fishman (mfishman@calarts.edu, (626) 463-3100).

## Learning objectives

By the end of this lecture, students should be able to:

- Explain what responsive design is: building one page that adapts its layout to whatever screen it lands on.
- Write a media query — a block of CSS that only applies when the screen meets a condition.
- Identify the parts of a media query (`@media`, media type, condition, styles).
- Choose breakpoints and understand the three common device ranges.
- Preview a page across devices using Chrome DevTools, the Xcode Simulator, and Safari.
- Explain why simulators aren't a substitute for testing on a real phone.
- Describe what a CSS framework provides, and name Bootstrap and Material-UI.

## Key terms

- **Responsive design** — building one page that adapts its layout to whatever screen it lands on.
- **Media query** — a block of CSS that only applies when the screen meets a condition (e.g. viewport ≤600px).
- **@media** — the keyword that begins a media query.
- **Media type `screen`** — the media type; almost always `screen` (vs `print`).
- **max-width / min-width** — the condition of a media query; `max-width: 600px` means apply when the viewport is ≤600px.
- **Breakpoint** — the width at which a media query kicks in.
- **The three device ranges** — Smartphone (max-width 767px), Tablet (768px–1023px), Desktop (min-width 1024px).
- **DevTools (Chrome DevTools)** — built into Chrome; emulate devices; free and cross-platform.
- **Xcode Simulator** — Apple's virtual iPhone & iPad; preview in Simulator Safari; macOS only.
- **Safari** — the default browser on iOS & macOS; dev tools for real-device debugging.
- **CSS framework** — a pre-built library of styles and components (grids, buttons, forms, navigation) that make it faster to build responsive, consistent pages.
- **Bootstrap** — by Twitter; responsive, mobile-first; flexible grid system; ready-made components; free & open-source.
- **Material-UI** — by Google; implements Material Design; consistent look across platforms; works with React, Angular, Vue; free & open-source.

## Lesson flow

**Slide 1 — Title.** "Responsive Web Design."

**Slide 2 — One site. Every screen.** People visit on phones, tablets, laptops, giant monitors. A layout that fills a laptop will overflow a phone. Responsive design is building one page that adapts its layout to whatever screen it lands on.

**Slide 3 — Media queries.** A block of CSS that only applies when the screen meets a condition (e.g. viewport ≤600px). Write default styles once, then add media queries to adjust as the screen gets smaller/larger.

**Slide 4 — Anatomy.**

```css
@media screen and (max-width: 600px) { body { font-size: 14px; } }
```

- `@media`: the keyword that begins a media query.
- `screen`: the media type — almost always screen (vs print).
- `(max-width: 600px)`: the condition — apply when viewport ≤600px; that width is a breakpoint.
- `{ … }`: the styles used when the condition is true.

**Slide 5 — Example.**

```css
body { font-size: 16px; }
```

```css
@media only screen and (max-width: 600px) { body { font-size: 14px; } }
```

Above the breakpoint the default 16px applies; at ≤600px the query shrinks text to 14px.

**Slide 6 — Breakpoints.**

- 📱 Smartphone: max-width 767px
- 📋 Tablet: 768px–1023px
- 🖥 Desktop: min-width 1024px

`// note` — common starting points, not hard rules. Set breakpoints where YOUR layout starts to break.

**Slide 7 — Testing.** Three ways to preview mobile:

- Chrome DevTools — built into Chrome, emulate devices, free/cross-platform.
- Xcode Simulator — Apple's virtual iPhone & iPad, preview in Simulator Safari, macOS only.
- Safari — default browser on iOS & macOS, dev tools for real-device debugging.

`// golden rule` — simulators are great, but nothing beats testing on a real phone.

**Slide 8 — Chrome DevTools.**

- Open: right-click → Inspect, or F12.
- Toggle device toolbar: Cmd/Ctrl + Shift + M.
- Panels: Elements (inspect & live-edit HTML/CSS), Console (debug JS), Audits/Lighthouse (find performance issues).
- Emulating devices/sizes is the single most useful feature for responsive layouts.

**Slide 9 — Xcode Simulator.** Apple's dev environment for macOS; includes the iOS Simulator (virtual iPhone/iPad). Install Xcode → Open Developer Tool ▸ Simulator → choose device & iOS version → browse in the Simulator's Safari. It's virtual — some features (geolocation, device APIs) may not work; not a substitute for a real device.

**Slide 10 — Real devices.** Emulators get you ~90%; screen sizes, resolutions, touch, and performance behave differently on actual hardware. Test on a variety of devices; use real devices whenever you can; cover different sizes/resolutions.

**Slide 11 — CSS frameworks.** A pre-built library of styles and components (grids, buttons, forms, navigation) that make it faster to build responsive, consistent pages. Drop in ready-made, tested pieces and customize.

**Slide 12 — Bootstrap & Material.**

- Bootstrap (by Twitter): responsive, mobile-first; flexible grid system; ready-made components (forms, buttons, modals, navbars); free & open-source.
- Material-UI (by Google): implements Material Design; consistent look across platforms; works with React, Angular, Vue; free & open-source.

`// both` give you a polished starting point — then you customize.

**Slide 13 — Recap.** Chips: responsive design, @media queries, max-width/min-width, breakpoints, phone/tablet/desktop, Chrome DevTools, Xcode Simulator, Safari debugging, Bootstrap, Material-UI.

`// the big idea` — build once, adapt everywhere. Set breakpoints where your layout breaks, and always test on real screens.

**Slide 14 — Homework: "Make your site adapt."** Add a media query to your project — shrink text or stack columns on small screens. Open Chrome DevTools (Cmd+Shift+M) and preview it across devices. Fix anything that overflows or breaks on phone width. Curious? Explore a CSS framework like Bootstrap. Closing: keep testing on real screens.

## Discussion prompts

- **(Slide 6 `// note`)** The breakpoints (smartphone 767px, tablet 768–1023px, desktop 1024px) are common starting points, not hard rules. Where should you actually set breakpoints? Set them where YOUR layout starts to break.
- **(Slide 7 `// golden rule`)** Simulators are great, but nothing beats testing on a real phone. Why is that?
- **(Slide 12 `// both`)** Both Bootstrap and Material-UI give you a polished starting point — then you customize.
- **(Slide 13 `// the big idea`)** Build once, adapt everywhere. Set breakpoints where your layout breaks, and always test on real screens.

## Watch out for

Only what the slides flag:

- Breakpoints go where YOUR layout breaks — the listed sizes are common starting points, not hard rules.
- Simulators/emulators get you ~90%; test on real hardware. Screen sizes, resolutions, touch, and performance behave differently on actual devices, and some features (geolocation, device APIs) may not work in the Simulator.

## Homework to assign

Assign **"Make your site adapt"** (slide 14):

1. Add a media query to your project — shrink text or stack columns on small screens.
2. Open Chrome DevTools (Cmd+Shift+M) and preview it across devices.
3. Fix anything that overflows or breaks on phone width.
4. Curious? Explore a CSS framework like Bootstrap.

Closing reminder for students: keep testing on real screens. (Full details in `assignment.md`.)

## Looking ahead

Keep reinforcing the habit that carries this week: keep testing on real screens.
