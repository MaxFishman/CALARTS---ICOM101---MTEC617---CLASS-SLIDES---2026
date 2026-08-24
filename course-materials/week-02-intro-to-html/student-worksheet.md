# Week 02 Worksheet — Introduction to HTML

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 02 — Introduction to HTML**
> _Student Worksheet_

Work through these exercises using only the tags we covered this week. Take your time, and remember: HTML is the skeleton of every web page — you're learning to build structure. The answer key is at the bottom, but try each one first.

## Key terms

Match each term on the left to its definition on the right.

| Term | | Definition |
| --- | --- | --- |
| 1. Markup | | A. Text that links to other text — hyperlinks |
| 2. Raw text | | B. A nested element inside another element |
| 3. HyperText | | C. A language that defines the structure & presentation of raw text |
| 4. Element | | D. Plain text that the computer interprets when wrapped in HTML elements |
| 5. Attribute | | E. An opening tag, its content, and its closing tag together |
| 6. Child | | F. Extra info in the opening tag, written as a name and a value |

## Anatomy

**a.** Label the three parts of this element:

```
<p>Hello World!</p>
```

- `<p>` is the __________ tag
- `Hello World!` is the __________
- `</p>` is the __________ tag

**b.** In this opening tag, label the name and the value:

```
<div id="intro">
```

- `id` is the __________
- `"intro"` is the __________

## Read & write the code

1. Write a bulleted (unordered) list of 3 groceries using `<ul>` and `<li>`.

2. Write an ordered list of 3 steps using `<ol>` and `<li>`.

3. Write an anchor (`<a>`) that links to `https://w3schools.com` with the visible text "Visit W3Schools".

4. Write an `<img>` tag with both required attributes: a `src` and an `alt`.

5. Which tag makes text **bold**? Which tag makes text _italic_?

6. Fix this code — a `<ul>` shouldn't hold raw text directly:

```
<ul>Limes Tortillas Chicken</ul>
```

## Short answer

**a.** What does "HyperText" mean?

**b.** What's the difference between a block element like `<p>` and an inline element like `<span>`?

**c.** Why would you use a `<div>`?

## Try it

Write a tiny one-section HTML page. Put everything inside a `<body>`, then inside it place a `<div>` with an `id`. Inside the div, add one `<h1>`, one `<p>` (with a `<span>` somewhere inside it), and an `<a>` link with an `href`. Indent two spaces per nesting level.

---

## Answer key

**Key terms:** 1-C, 2-D, 3-A, 4-E, 5-F, 6-B

**Anatomy a:**
- `<p>` is the **opening** tag
- `Hello World!` is the **content**
- `</p>` is the **closing** tag

**Anatomy b:**
- `id` is the **name**
- `"intro"` is the **value**

**Read & write the code:**

1. Example:
```
<ul><li>Limes</li><li>Tortillas</li><li>Chicken</li></ul>
```

2. Example:
```
<ol><li>Preheat oven to 350°.</li><li>Mix flour & salt.</li><li>Cream butter & sugar.</li></ol>
```

3.
```
<a href="https://w3schools.com">Visit W3Schools</a>
```

4. Example:
```
<img src="img_girl.jpg" alt="Girl in a jacket">
```
Both `src` (the path) and `alt` (text shown if it can't load, and read aloud by screen readers) are required.

5. `<strong>` marks important text — rendered bold. `<em>` adds emphasis — usually italic.

6. Every item needs its own `<li>` — the `<ul>` shouldn't hold raw text directly:
```
<ul><li>Limes</li><li>Tortillas</li><li>Chicken</li></ul>
```

**Short answer:**

**a.** HyperText means text that links to other text — hyperlinks.

**b.** `<p>` holds a block of plain text, while `<span>` wraps a short inline piece on the same line so you can target it on its own.

**c.** `<div>` is short for "division." It has no visual look of its own, but it groups elements into sections so you can style them together later.

**Try it — example answer:**
```
<body>
  <div id="intro">
    <h1>My First Page</h1>
    <p>Hello, this is <span>my</span> page.</p>
    <a href="https://w3schools.com">Visit W3Schools</a>
  </div>
</body>
```
