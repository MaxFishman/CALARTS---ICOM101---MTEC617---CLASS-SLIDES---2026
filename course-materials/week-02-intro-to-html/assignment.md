# Week 02 Homework — Introduction to HTML

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 02 — Introduction to HTML**
> _Homework Assignment_

## Overview

This week you learned that HTML is the skeleton of every web page — it gives structure to content like images, text, and video. Now it's time to build your own page by hand. Don't worry about how it looks yet (that's next week, when we style it all with CSS). For now, your goal is to practice using the HTML elements we covered and to get comfortable with tags, nesting, and attributes.

You've got this. Take it one tag at a time.

## What you'll practice

- Placing content inside the `<body>` so it reaches the screen
- Using headings `<h1>`–`<h6>` in order, largest to smallest
- Grouping elements with a `<div>` and labeling it with an `id`
- Writing paragraphs with `<p>` and inline pieces with `<span>`
- Marking text with `<strong>` (bold) and `<em>` (italic)
- Forcing a line break with `<br>`
- Building an unordered list (`<ul>`/`<li>`) and an ordered list (`<ol>`/`<li>`)
- Using a semantic element like `<article>`, `<figure>`, or `<nav>`
- Making a hyperlink with `<a>` and its `href` attribute
- Placing an image with `<img>` and its `src` and `alt` attributes

## The assignment

Hand-write a small HTML page about a topic you like (a hobby, a favorite place, a recipe — your choice). Write it by hand so the tags sink in. Follow these numbered steps in order.

1. Start with an opening `<body>` and a closing `</body>` tag. Remember: only what's in the body reaches the screen, so all of your content goes between these two tags.

2. Add one `<h1>` as the main heading of your page. Use `<h1>` only once.

3. Add at least two more headings from `<h2>`–`<h6>` as subheadings, ordered largest to smallest.

4. Create a `<div>` to group a section of your page together, and give it an `id` attribute (for example, `<div id="intro">`). The `id` goes in the opening tag.

5. Inside that `div`, write at least two paragraphs using `<p>`.

6. In one of your paragraphs, wrap a short inline piece of text in a `<span>` so it stays on the same line.

7. Somewhere in your text, use `<strong>` to mark something important (it renders bold) and `<em>` to add emphasis (usually italic).

8. Use a `<br>` to force a line break inside a paragraph. Remember `<br>` has only an opening tag — no closing tag.

9. Add an unordered list using `<ul>` with three `<li>` items. Every item needs its own `<li>` — the `<ul>` shouldn't hold raw text directly.

10. Add an ordered list using `<ol>` with three `<li>` items (great for steps or a ranking).

11. Wrap a self-contained part of your page in one semantic element: `<article>`, `<figure>` (pair it with `<figcaption>`), or `<nav>`.

12. Add a hyperlink using `<a>` with an `href` attribute pointing to a real URL — for example `<a href="https://w3schools.com">Visit W3Schools</a>`. Remember: no href, no hyperlink.

13. Add an image using `<img>` with both required attributes: `src` (the path) and `alt` (text shown if it can't load, and read aloud by screen readers) — for example `<img src="img_girl.jpg" alt="Girl in a jacket">`.

14. Indent your code two spaces per nesting level so the hierarchy of parents and children is easy to read.

## Submission

- Save your work as a single `.md` or `.txt` file (or a `.html` file if you'd like) containing your hand-written HTML.
- Name the file `week02-yourname` (for example, `week02-jordan`).
- Submit it before the start of next class.
- Questions? Email Max Fishman at mfishman@calarts.edu or call (626) 463-3100.

## How it's graded

This is a light rubric — the goal is practice, not perfection. Each required element is worth points for being present and used correctly.

| Requirement | Points |
| --- | --- |
| `<body>` wraps all content | 8 |
| One `<h1>` used once, plus `<h2>`–`<h6>` subheadings in order | 10 |
| A `<div>` with an `id` attribute grouping a section | 10 |
| At least two `<p>` paragraphs | 8 |
| A `<span>` used inline inside a paragraph | 8 |
| `<strong>` and `<em>` each used | 8 |
| A `<br>` line break used correctly (opening tag only) | 6 |
| A `<ul>` with three `<li>` items (no raw text in the `<ul>`) | 10 |
| An `<ol>` with three `<li>` items | 10 |
| One semantic element (`<article>`, `<figure>`, or `<nav>`) | 8 |
| An `<a>` with a valid `href` | 8 |
| An `<img>` with both `src` and `alt` | 8 |
| **Total** | **100** |
