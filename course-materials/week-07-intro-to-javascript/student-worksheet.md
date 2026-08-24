# Week 07 Worksheet — Introduction to JavaScript

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 07 — Introduction to JavaScript**
> _Student Worksheet_

Work through these on your own, then check yourself against the answer key at the bottom. Everything here comes straight from this week's lecture.

## Predict the output

For each line, write what `console.log` prints.

1. `console.log(11 % 3)` → __________
2. `console.log('hi' + 'ya')` → __________
3. `console.log('Hello'.length)` → __________
4. `console.log('hello'.toUpperCase())` → __________
5. With `const myPet = 'armadillo';`, what does this print?
   `` console.log(`I own a pet ${myPet}.`) `` → __________

## Data types

1. Name the 7 data types.

   1. ______  2. ______  3. ______  4. ______  5. ______  6. ______  7. ______

2. Which of them are primitive?

   __________________________________________________

## Read & write the code

1. Declare a variable with `let`, then reassign it.

   ```js


   ```

2. Write a template literal that builds a sentence from a variable.

   ```js


   ```

3. Write a button with a click event that logs a message.

   ```html


   ```

4. `.length` is a property and `.toUpperCase()` is a method. Which one needs parentheses `()`?

   __________________________________________________

## Short answer

1. What does `console.log` do?

   __________________________________________________

2. What's the difference between `let` and `const`?

   __________________________________________________

3. What does `typeof` do?

   __________________________________________________

4. What do jQuery's `$()` selectors mirror?

   __________________________________________________

## Try it

A mini version of the homework. In a `<script>`:

- `console.log()` a greeting.
- Add a button with a click event that logs a message.

```html


```

## Answer key

**Predict the output**
1. `2` (the remainder of 11 ÷ 3)
2. `'hiya'`
3. `5`
4. `'HELLO'`
5. `'I own a pet armadillo.'`

**Data types**
1. Number, String, Boolean, Null, Undefined, Symbol, Object.
2. The first 6 are primitive: Number, String, Boolean, Null, Undefined, Symbol.

**Read & write the code**
1. Example:
   ```js
   let w = 4;
   w += 1;
   console.log(w); // 5
   ```
2. Example:
   ```js
   const myPet = 'armadillo';
   console.log(`I own a pet ${myPet}.`);
   ```
3. Example (either way works):
   ```html
   <button onclick="alert('Hi!')">Click</button>
   ```
   ```js
   const btn = document.getElementById('hi');
   btn.addEventListener('click', () => {
     console.log('Hello World!');
   });
   ```
4. The method needs parentheses: `.toUpperCase()`. A property like `.length` does not.

**Short answer**
1. `console.log(...)` prints whatever's in the parentheses to the console (a panel in DevTools that shows messages for developers).
2. `let` can change later; `const` is constant, and reassigning it throws an error.
3. `typeof` tells you a value's data type.
4. jQuery's `$()` selectors mirror CSS selectors.

**Try it** — example:
```html
<script>
  console.log('Hello World!');
  const btn = document.getElementById('hi');
  btn.addEventListener('click', () => {
    console.log('Hello World!');
  });
</script>
<button id="hi">Click</button>
```
