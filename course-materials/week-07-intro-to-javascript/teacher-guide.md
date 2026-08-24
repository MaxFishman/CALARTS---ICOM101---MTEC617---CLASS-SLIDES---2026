# Week 07 Teacher Guide — Introduction to JavaScript

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 07 — Introduction to JavaScript**
> _Teacher Guide_

## At a glance

- **Course:** Intro to Web Development — ICOM101 / MTEC617, CalArts, Spring 2026
- **Instructor:** Max Fishman (mfishman@calarts.edu, (626) 463-3100)
- **Week:** 07 of 9 — Introduction to JavaScript
- **Format:** 17-slide lecture
- **Prerequisite:** Weeks 01–06
- **Big idea:** HTML gives structure, CSS gives style — JavaScript gives behavior. Today we start with the building blocks of a real programming language.
- **Ends with:** A homework checklist on slide 17 ("Write some JavaScript").

## Learning objectives

By the end of the lecture, students can:

- Print messages to the console with `console.log()` and end statements with a `;`.
- Write single-line (`//`) and multi-line (`/* … */`) comments.
- Name the 7 data types and identify which are primitive.
- Use arithmetic operators, including `%` (modulo).
- Concatenate strings with `+`, watching their spaces.
- Use the dot operator to reach a property or call a method.
- Use the `Math` object with `Math.random()` and `Math.floor()`.
- Declare variables with `let`, `const`, and `var`, and reassign with `+=`, `++`, `--`.
- Build strings with template literals and check a value's type with `typeof`.
- Respond to events with an inline attribute or `addEventListener`.
- Select elements and run animations with jQuery.

## Key terms

- **`console.log()`** — a method that prints whatever's in the parentheses to the console (a panel in DevTools that shows messages for developers).
- **Comments (`//` and `/* */`)** — notes for humans; the code doesn't run. `//` comments one line; `/* … */` wraps many.
- **The 7 data types** — Number, String, Boolean, Null, Undefined, Symbol, Object.
- **Arithmetic operators** — `+` add, `-` subtract, `*` multiply, `/` divide, `%` remainder (modulo).
- **String concatenation** — joining strings with the `+` operator.
- **Dot operator (`.`)** — reaches into a value; a **property** holds info (`.length`), a **method** does something and needs `()` (`.toUpperCase()`).
- **The `Math` object** — a built-in object full of methods; `Math.random()` gives 0–1, `Math.floor()` rounds down.
- **Variables (`let` / `const` / `var`)** — `let` can change, `const` is constant, `var` is the old pre-2015 way (prefer `let`/`const`).
- **Assignment operator (`=`)** — assigns a value to a variable.
- **Reassignment (`+=`, `++`, `--`)** — `+=`, `-=`, `*=`, `/=` update in place; `++` and `--` add/subtract 1.
- **Template literals** — a string in backticks with values inserted via `${ }`.
- **`typeof`** — tells you a value's data type.
- **Events & `addEventListener`** — an event is something that happens (a click, hover, or key press) that can trigger code; `addEventListener` is the cleaner way to respond.
- **jQuery `$()` selectors** — jQuery is a JavaScript library that simplifies working with the page; its `$()` selectors mirror CSS selectors.
- **jQuery animations** — ready-made animations: `fadeIn()`, `fadeOut()`, `slideUp()`, `slideDown()`, `animate()`.

## Lesson flow

**Slide 1 — Title: JavaScript.** Open with a live one-liner.
```html
<script>console.log('hello, world');</script>
```

**Slide 2 — What is JS.** HTML gives structure, CSS gives style — JavaScript gives behavior: things that happen and change after the page loads. Clicks, hovers, key presses, animations, live updates. It's a real programming language, so today we start with its building blocks.

**Slide 3 — The console.**
```js
console.log(5);
console.log('Hello World!');
```
Outputs `5` and `'Hello World!'`. The console is a panel (in DevTools) that shows messages for developers. `console.log(...)` prints whatever's in the parentheses. End statements with a `;`.

**Slide 4 — Comments.**
```js
// a single-line comment
console.log(5); // …or after some code
/* a multi-line comment
none of this runs */
```
Comments are for humans. `//` comments one line; `/* … */` wraps many.

**Slide 5 — Data types.** 7 types:
- **Number** — `4`, `23.42` — any number, decimals too
- **String** — `'hello'` — text in quotes
- **Boolean** — `true`/`false` — a yes/no switch
- **Null** — `null` — intentionally empty
- **Undefined** — `undefined` — no value yet
- **Symbol** — a unique id — advanced, later
- **Object** — `{ … }` — a collection of related data

The first 6 are primitive — the most basic types.

**Slide 6 — Arithmetic.**
```js
console.log(3 + 4);
console.log(9 / 3);
console.log(11 % 3);
```
Outputs `7`, `3`, `2` (remainder). Operators: `+` add, `-` subtract, `*` multiply, `/` divide, `%` remainder (modulo). `11 % 3` is `2`.

**Slide 7 — Concatenation.**
```js
console.log('hi' + 'ya');
console.log('I love to ' + 'code.');
```
Outputs `'hiya'`, `'I love to code.'`. The `+` operator on strings concatenates. Watch your spaces: `'love to '` keeps the trailing space.

**Slide 8 — Properties & methods.**
```js
console.log('Hello'.length);        // 5
console.log('hello'.toUpperCase());  // 'HELLO'
console.log('Hey'.startsWith('H'));  // true
```
The `.` is the dot operator. A property holds info (`.length`); a method does something and needs `()` (`.toUpperCase()`). `console.log()` is a method too.

**Slide 9 — The Math object.**
```js
Math.random();                  // 0–1
Math.floor(Math.random() * 50); // a whole number 0–49
```
`Math` is a built-in object full of methods. `Math.floor()` rounds down.

**Slide 10 — Variables.**
```js
let myName = 'Arya';
console.log(myName); // Arya
```
`let` — value can change later (everyday choice). `const` — value is constant (reassigning throws an error). `var` — the old pre-2015 way; prefer `let`/`const`. Names use camelCase, can't start with a number, case-sensitive. `=` is the assignment operator.

**Slide 11 — Reassigning.**
```js
let w = 4;
w += 1;
console.log(w); // 5

let a = 10;
a++;
a--;
```
Use `let` when a value needs to change; `const` can't be reassigned. Shortcuts: `+=`, `-=`, `*=`, `/=` update in place; `++` and `--` add/subtract 1. A `let` with no value starts as `undefined`.

**Slide 12 — Template literals.**
```js
const myPet = 'armadillo';
console.log(`I own a pet ${myPet}.`);
console.log(typeof myPet);
```
Outputs `'I own a pet armadillo.'`, `'string'`. Wrap a string in backticks and insert values with `${ }` — cleaner than gluing with `+`. `typeof` tells you a value's data type.

**Slide 13 — Events.**
```html
<button onclick="alert('Hi!')">Click</button>
```
```js
const btn = document.getElementById('hi');
btn.addEventListener('click', () => {
  console.log('Hello World!');
});
```
An event is something that happens — a click, hover, or key press — that can trigger your code. Two ways: an inline attribute, or `addEventListener` (the cleaner way).

**Slide 14 — jQuery select.** Add jQuery in `<head>`, then:
```js
$('p')            // all <p>
$('.my-class')    // class
$('#my-id')       // id
$('div.my-class p') // combined
$('#my-id').hide();
```
jQuery is a JavaScript library that simplifies working with the page. Its `$()` selectors mirror CSS selectors.

**Slide 15 — jQuery animate.**
```js
$('button').click(function() {
  $(this).fadeOut('slow');
});
```
Also `fadeIn()`, `slideUp()`, `slideDown()`, `animate()`. jQuery bundles ready-made animations.

**Slide 16 — Recap.** Chips: `console.log()`, comments, 7 data types, `+ - * / %`, concatenation, `.length`, `.methods()`, `Math`, `let`/`const`, `+= ++ --`, template literals, `typeof`, events, jQuery `$()`.

**Slide 17 — Homework: "Write some JavaScript."** See "Homework to assign" below.

## Discussion prompts

Use the slide-16 "big idea" note verbatim to anchor the closing discussion:

> // the big idea — variables store data, methods act on it, and events run your code in response to the user. This is the foundation everything else builds on.

Ask students to point to where each part (store data / act on it / respond to the user) showed up in today's code.

## Watch out for

Only the things the slides flag:

- End statements with a `;`.
- Watch your spaces in concatenation so words don't collide (`'love to '` keeps its trailing space).
- A method needs `()` but a property doesn't (`.toUpperCase()` vs `.length`).
- Variable names use camelCase, can't start with a number, and are case-sensitive.
- A `let` with no value starts as `undefined`.
- `const` can't be reassigned (reassigning throws an error).

## Homework to assign

Assign slide 17, "Write some JavaScript":

- Add a `<script>` to your project and `console.log()` a greeting.
- Make a variable with `let`, then reassign it.
- Use a template literal to build a sentence from a variable.
- Add a button with a click event that logs a message.
- Curious? Load jQuery and `fadeOut()` an element on click.

## Looking ahead

Leave students with the closing line: open DevTools and watch it run.
