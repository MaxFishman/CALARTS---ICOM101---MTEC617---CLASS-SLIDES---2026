# Week 05 Worksheet — Position, Color & Motion

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 05 — Position, Color & Motion**
> _Student Worksheet_

Work through these on your own — three acts: place it, paint it, move it. Check your answers against the key at the bottom only after you've tried.

## Position

**1. Match each `position` value to its behavior.** Draw a line or write the letter.

| Value | | Behavior |
| --- | --- | --- |
| `relative` | ___ | A. Locks to a spot on the screen and ignores scrolling. |
| `fixed` | ___ | B. Positions the element relative to its own default spot; the space it used to occupy is left behind. |
| `sticky` | ___ | C. Scrolls normally until it hits your offset, then sticks there until its parent scrolls past. |

**2.** Which `position` value pins an element to the screen and ignores scrolling? _______________

## Read & write the code

Write the CSS rule for each. (You choose the selector name.)

**3.** A box with `position: relative`, moved 50px down and 120px right.
```css
```

**4.** A fixed header pinned to the top-left corner (`top: 0` and `left: 0`).
```css
```

**5.** Text in the foreground colored red on a gold background.
```css
```

**6.** A background gradient that blends from left to right, red into blue.
```css
```

**7.** A link that changes color when the pointer is over it (a `:hover` color change).
```css
```

**8.** A `transition` shorthand that animates `color` over 1.5s with `linear` timing after a 0.5s delay.
```css
```

## Short answer

**9.** When two positioned boxes overlap, what does `z-index` control?

**10.** `opacity` runs from 0 to 1. What do 0 and 1 each mean?

**11.** A transition controls four things. Name them.

## Try it

A mini version of the homework. In your project (or a scratch file):

- Add a **sticky header** — one that scrolls normally, then sticks when it hits its offset.
- Add a link with a **hover color change**, and give it a **transition** so the change eases in smoothly instead of snapping.

Write your CSS here:
```css
```

---

## Answer key

**1.** `relative` → B; `fixed` → A; `sticky` → C.

**2.** `fixed`.

**3.**
```css
.green-box {
  position: relative;
  top: 50px;
  left: 120px;
}
```

**4.**
```css
.title {
  position: fixed;
  top: 0px;
  left: 0px;
}
```

**5.**
```css
h1 {
  color: red;
  background-color: gold;
}
```

**6.**
```css
background: linear-gradient(to right, red, blue);
```

**7.**
```css
a:hover {
  color: goldenrod;
}
```
(Any color change on `:hover` is correct — for example changing from `purple` to `goldenrod`.)

**8.**
```css
transition: color 1.5s linear 0.5s;
```
(Order: property duration timing delay. Remember: to set a delay you must also set a duration — the browser reads the first time value as the duration.)

**9.** `z-index` sets the depth of overlapping positioned boxes — a higher number sits in front.

**10.** 0 = fully invisible; 1 = fully solid. (0.5 is half-transparent.)

**11.** property (which CSS property animates), duration (how long it takes), timing (how it accelerates), and delay (how long to wait before it starts).

**Try it — example answer:**
```css
.header {
  position: sticky;
  top: 0px;
}
a {
  color: purple;
  transition: color 0.4s ease;
}
a:hover {
  color: goldenrod;
}
```
