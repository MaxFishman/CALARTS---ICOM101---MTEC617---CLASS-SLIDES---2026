# Week 07 Homework — Introduction to JavaScript

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 07 — Introduction to JavaScript**
> _Homework Assignment_

## Overview

This week you met JavaScript — the language that gives a web page behavior: things that happen and change after the page loads, like clicks, hovers, key presses, animations, and live updates. HTML gives structure, CSS gives style, and JavaScript gives behavior.

For this homework you'll write some JavaScript of your own. You'll add a `<script>` to your project and try out the building blocks we covered: printing to the console, making a variable, building a sentence with a template literal, and responding to a click. Keep it simple — the goal is to see your code run.

## What you'll practice

- Printing a message with `console.log()`
- Making a variable with `let` and reassigning it
- Building a sentence with a template literal
- Adding a button with a click event that logs a message
- (Optional) Loading jQuery and using `fadeOut()`

## The assignment

Add a `<script>` to your project and work through the checklist below. Everything here comes straight from the lecture — there's nothing new to learn.

1. **Add a `<script>` and `console.log()` a greeting.** Put a `<script>` in your project and use `console.log()` to print a greeting message. Remember to end statements with a `;`.

2. **Make a variable with `let`, then reassign it.** Declare a variable using `let` (names use camelCase, can't start with a number, and are case-sensitive). Then give it a new value later. `let` is for values that can change.

3. **Use a template literal to build a sentence from a variable.** Wrap a string in backticks and insert your variable with `${ }` to build a sentence — cleaner than gluing pieces together with `+`.

4. **Add a button with a click event that logs a message.** Add a button, and when it's clicked, log a message. You can use `addEventListener` (the cleaner way) or an inline `onclick` attribute.

5. **Curious? (Optional)** Load jQuery in your `<head>`, then make an element `fadeOut()` when it's clicked.

## Submission

Submit your project files containing your `<script>`. Make sure your greeting, your variable, your template literal, and your button click all work. Open DevTools and watch it run before you submit.

## How it's graded

This is a light, practice-focused assignment. Credit is for showing each piece working:

| Item | What we're looking for |
| --- | --- |
| `console.log()` greeting | A greeting prints to the console |
| Variable with `let` + reassign | A `let` variable is declared and given a new value |
| Template literal | A sentence is built from a variable using backticks and `${ }` |
| Button click event | A button click logs a message |
| jQuery `fadeOut()` (optional) | Bonus: an element fades out on click |
