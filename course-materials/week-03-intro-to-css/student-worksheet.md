# Week 03 Worksheet — Introduction to CSS

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 03 — Introduction to CSS**
> _Student Worksheet_

HTML builds it, CSS makes it beautiful — use this worksheet to practice writing rulesets, working the box model, and styling type. Try each section on your own before checking the answer key at the bottom.

## Anatomy of a ruleset

Label each part of this ruleset. Fill in the blanks with: **selector**, **declaration block**, **declaration**, **property**, **value**.

```css
h1 { color: blue; }
```

- `h1` is the ______________
- `{ color: blue; }` is the ______________
- `color: blue;` is the ______________
- `color` is the ______________
- `blue` is the ______________

## The box model

Every element lives in a box. Put these four layers in order **from inside out**:

`border` · `margin` · `content` · `padding`

1. ______________ (innermost)
2. ______________
3. ______________
4. ______________ (outermost)

- Which layer is space **inside** the box? ______________
- Which layer is space **outside** the box? ______________

## Read & write the code

Use ONLY properties from this week.

1. Write a rule that gives every `<p>` a coral border (3px, solid).

2. Center a box that is 400px wide using a `.headline` class.

3. Make a perfect circle with a `.dot` class using border-radius.

4. Write the `<link>` tag that links an external stylesheet at `styles/style.css`. (Remember where it lives and that it's self-closing.)

5. Write the CSS reset rule using the universal selector.

6. Give `<h1>` a serif font stack with a fallback, ending in a generic keyword. (Wrap any multi-word name in quotes.)

## Short answer

1. Name the **three** places CSS can go, and say which is best practice.

2. What does **margin collapse** do to two stacked vertical margins?

3. What does `overflow: scroll;` do?

## Try it

A mini version of the homework. On a small project (fork last week's, or start fresh):

- Add CSS using the box model: padding, margin, or a border.
- Change an element's color or background-color.
- Change an element's font from the default with `font-family`.
- Use at least one `class` attribute to style some HTML selectively.

---

## Answer key

**Anatomy of a ruleset**

- `h1` is the **selector**
- `{ color: blue; }` is the **declaration block**
- `color: blue;` is the **declaration**
- `color` is the **property**
- `blue` is the **value**

**The box model** (inside out)

1. **content** (innermost)
2. **padding**
3. **border**
4. **margin** (outermost)

- Space inside: **padding**
- Space outside: **margin**

**Read & write the code**

1.
```css
p { border: 3px solid coral; }
```

2.
```css
.headline { width: 400px; margin: 0 auto; }
```

3.
```css
.dot { border-radius: 50%; }
```

4.
```html
<link href="styles/style.css" rel="stylesheet">
```
(Lives inside `<head>` and is self-closing.)

5.
```css
* { margin: 0; padding: 0; }
```

6.
```css
h1 { font-family: Georgia, 'Times New Roman', serif; }
```

**Short answer**

1. Inline (`<p style="color:red;">Hi</p>` — quick, rarely used); internal (`<style>` inside `<head>` — better, still not best); external (a separate `.css` file). **External is best practice** — HTML stays clean, CSS maintainable.

2. Vertical margins collapse — the browser keeps the **LARGER** of the two. (Stacked 10px & 30px sit 30px apart.) Padding never collapses.

3. `overflow: scroll;` adds a scrollbar (versus visible → spills outside, the default; hidden → clipped/hidden).
