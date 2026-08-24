# Week 02 Teacher Guide — Introduction to HTML

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 02 — Introduction to HTML**
> _Teacher Guide_

## At a glance

- **Course:** Intro to Web Development (ICOM101 / MTEC617), CalArts, Spring 2026
- **Instructor:** Max Fishman — mfishman@calarts.edu — (626) 463-3100
- **Week:** 02 of 9 — Introduction to HTML
- **Format:** 18-slide lecture
- **Prerequisite:** Week 01
- **Big idea:** HTML is the skeleton of every web page — it gives structure to content. It's usually the first language developers, designers, and marketers learn.

## Learning objectives

By the end of this week, students should be able to:

- Explain what HTML is and why it's the structure of a web page
- Break down the anatomy of an element (opening tag, content, closing tag)
- Place content inside the `<body>` so it reaches the screen
- Understand hierarchy — parents, children, and nesting
- Use headings `<h1>`–`<h6>`, `<div>`, `<p>`, and `<span>`
- Add attributes (name + value), including `id`
- Distinguish block from inline content
- Mark text with `<strong>` and `<em>`, and break lines with `<br>`
- Build unordered (`<ul>`/`<li>`) and ordered (`<ol>`) lists
- Use semantic tags (`<article>`, `<figure>`, `<nav>`)
- Create hyperlinks with `<a href>` and images with `<img>` (`src` + `alt`)

## Key terms

Use the slides' own wording:

- **Element:** An opening tag, its content, and its closing tag together make one element.
- **Tag:** The markup that wraps content — an opening tag like `<p>` and a closing tag like `</p>`.
- **Opening / closing tag:** `<p>` is the opening tag; `</p>` is the closing tag.
- **Content:** The raw text (or other elements) between the opening and closing tags, e.g. `Hello World!`.
- **Attribute (name + value):** Extra info in the opening tag, written as name and value — e.g. `id` = name, `"intro"` = value.
- **id:** An attribute that labels a specific element — useful when you reuse an element and need to tell copies apart.
- **Hierarchy / parent / child / nesting:** A nested element is a child; the one around it is the parent. This set of relationships is hierarchy. Children can inherit styling from parents (more in CSS).
- **Block vs inline:** `<p>` holds a block of plain text; `<span>` wraps a short inline piece on the same line so you can target it on its own.
- **Semantic elements:** Tags like `<article>`, `<figure>`, and `<nav>` that don't look special in the browser but tell people, search engines, and assistive tech what each part means.
- **href:** The `<a>` tag's attribute that holds the destination URL — no href, no hyperlink.
- **src:** The `<img>` attribute holding the path to the image.
- **alt:** The `<img>` attribute with text shown if the image can't load — and read aloud by screen readers.

## Lesson flow

**Slide 1 — Title.** Introduce the topic: "Introduction to HTML."

**Slide 2 — The skeleton of every web page.** HTML gives structure to the content on a website — images, text, video. It's usually the first language developers, designers, and marketers learn.

**Slide 3 — HyperText Markup Language.** Break the name apart:
- Markup: A language that defines the structure & presentation of raw text.
- Raw text: The computer interprets plain text wrapped in HTML elements.
- HyperText: Text that links to other text — hyperlinks.

**Slide 4 — Anatomy.** Walk through the three parts of an element:
```
<p>Hello World!</p>
```
`<p>` is the opening tag; `Hello World!` is the content; `</p>` is the closing tag. Together they make one element.

**Slide 5 — The body.** Only what's in the body reaches the screen. Content lives between the opening `<body>` and closing `</body>`. Text, images, buttons — it all goes here.
```
<body>
  <p>What's up, doc?</p>
</body>
```

**Slide 6 — Hierarchy.** Parents, children, nesting. A nested element is a child; the one around it is the parent. This set of relationships is hierarchy — children can inherit styling from parents (more in CSS). Indent two spaces per level.
```
<body>
  <div>
    <h1>Why use divs?</h1>
    <p>A child of the div</p>
  </div>
</body>
```

**Slide 7 — Headings.** Six levels, largest to smallest: `<h1>` is the main heading (use once); `<h2>`–`<h6>` are subheadings ordered largest to smallest.
```
<h1>BREAKING NEWS</h1>
```

**Slide 8 — Divs.** Divide the page into sections. `<div>` is short for "division." It has no visual look of its own — but it groups elements so you can style them together later.
```
<body><div><h1>Why use divs?</h1><p>Great for grouping!</p></div></body>
```

**Slide 9 — Attributes.** Name + value. Attributes go in the opening tag. `id` labels a specific element — useful when you reuse an element and need to tell copies apart. Here `id` = name and `"intro"` = value.
```
<div id="intro"><h1>Introduction</h1></div>
```

**Slide 10 — Block vs inline.** `<p>` holds a block of plain text; `<span>` wraps a short inline piece (same line) so you can target it on its own.
```
<p><span>Self-driving cars</span> are anticipated to replace up to 2 million jobs.</p>
```

**Slide 11 — Em & strong.** `<strong>` marks important text — rendered bold; `<em>` adds emphasis — usually italic.
```
<p><strong>The Nile River</strong> is the <em>longest</em> river in the world.</p>
```

**Slide 12 — Line breaks.** `<br>` forces a line break; it has only an opening tag, no closing tag. Whitespace in your code doesn't move things on screen.

**Slide 13 — Unordered lists.** `<ul>` is the list; each item is an `<li>`. The `<ul>` shouldn't hold raw text directly — every item needs its own `<li>`.
```
<ul><li>Limes</li><li>Tortillas</li><li>Chicken</li></ul>
```

**Slide 14 — Ordered lists.** `<ol>` numbers each item — good for steps or a ranking.
```
<ol><li>Preheat oven to 350°.</li><li>Mix flour & salt.</li><li>Cream butter & sugar.</li></ol>
```

**Slide 15 — Semantic tags.**
- `<article>`: independent, self-contained content (forum post, blog post, news story).
- `<figure>`: self-contained media (illustrations, diagrams, photos, code listings); pair with `<figcaption>`.
- `<nav>`: a block of major navigation links; only for major nav.

// discuss — these don't look special in the browser, but they tell people, search engines, and assistive tech what each part means.

**Slide 16 — Links & href.** The `<a>` (anchor) tag makes a link; its `href` attribute is the destination URL — no href, no hyperlink.
```
<a href="https://w3schools.com">Visit W3Schools</a>
```

**Slide 17 — Images.** The `<img>` tag makes a holding space for an image it links to. Two required attributes: `src` (the path) and `alt` (text shown if it can't load — and read aloud by screen readers).
```
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```

**Slide 18 — Recap.** Review the tags covered: `<body>`, `<div>`, `<h1>–<h6>`, `<p>`, `<span>`, `<em>`, `<strong>`, `<br>`, `<ul>/<li>`, `<ol>`, `<article>`, `<figure>`, `<nav>`, `<a href>`, `<img>`. Up next: styling it all with CSS.

## Watch out for

Flag these common mistakes — each is called out in the slides:

- **`<br>` has only an opening tag** — there is no closing tag for it.
- **`<ul>` shouldn't hold raw text** — every item needs its own `<li>`.
- **`href` is required for a link** — no href, no hyperlink.
- **`<img>` needs both `src` and `alt`** — both attributes are required.
- **Indent two spaces per nesting level** so hierarchy stays readable.

## Homework to assign

Assign the Week 02 homework (`assignment.md`): students hand-write a small HTML page about a topic of their choice, using only the elements taught this week — `<body>`, one `<h1>` plus `<h2>`–`<h6>` subheadings, a `<div>` with an `id`, paragraphs with `<p>`, an inline `<span>`, `<strong>` and `<em>`, a `<br>`, a `<ul>`/`<li>` list, an `<ol>`/`<li>` list, one semantic element (`<article>`, `<figure>`, or `<nav>`), an `<a>` with `href`, and an `<img>` with `src` and `alt`. Grading follows the light rubric in the assignment.

## Looking ahead

Up next: styling it all with CSS.
