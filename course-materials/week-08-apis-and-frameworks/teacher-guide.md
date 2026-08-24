# Week 08 Teacher Guide — APIs & Frameworks

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 08 — APIs & Frameworks**
> _Teacher Guide_

## At a glance

- **Course:** Intro to Web Development — ICOM101 / MTEC617, CalArts, Spring 2026 (9-week course).
- **Instructor:** Max Fishman — mfishman@calarts.edu, (626) 463-3100.
- **This week:** Week 08 — APIs & Frameworks, an 11-slide lecture.
- **Prerequisite:** Weeks 01–07.
- **Focus:** Mostly conceptual. The aim is for students to understand what an API is, how the request/response flow works, and what frameworks give them — not to write framework code from scratch.
- **Deliverable:** Homework "Connect to the wider web" (slide 11).

## Learning objectives

By the end of the session students should be able to:

- Explain what an API is: a set of rules and tools that let two software applications communicate, without either knowing how the other is built inside.
- Trace the request/response flow from an app, through the API, to a service, and back.
- Name the three types of APIs (web, OS, library-based) with an example of each.
- State why APIs matter: reuse code, combine powers, collaborate and innovate, better experience.
- Define a framework and recognize the five in the lineup, including each one's language and whether it's front-end or back-end.

## Key terms

- **API (Application Programming Interface):** a set of rules and tools that let two software applications communicate — the interface between programs. One app can share data and functionality with another without either knowing how the other is built inside.
- **Request / response:** your app sends a **request** through the API; the service sends a **response** back. You use the result without ever seeing the other system's code.
- **Three types of APIs:**
  - **Web APIs** — let different web applications talk over the internet (e.g. Google Maps API).
  - **Operating System APIs** — give programs access to OS functions: files, network, hardware (e.g. file system access).
  - **Library-Based APIs** — expose the functions and resources of a specific software library (e.g. a charting library).
- **Framework:** a set of pre-built software components that give you a foundation for building web applications. Instead of wiring up everything yourself, you start from proven structure and build quickly on top of it.
- **The five frameworks (slides' own wording):**
  - **React** — JavaScript, library, **front-end**: reusable UI components; great for single-page apps (SPAs).
  - **Angular** — TypeScript, framework, **front-end**: large, complex front-ends; built-in routing, forms, dependency injection.
  - **Django** — Python, framework, **back-end**: "batteries included" — auth, admin panel, database handling built in.
  - **Flask** — Python, micro-framework, **back-end**: lightweight, few built-ins; ideal for simple apps or small APIs.
  - **Ruby on Rails** — Ruby, framework, **back-end**: "convention over configuration" — sensible defaults let you build fast.

## Lesson flow

1. **Title — "APIs & Frameworks" (GET /data).** Set the stage for the two big ideas of the week.
2. **What is an API.** An API is a set of rules and tools that let two software applications communicate — the interface between programs. One app can share data and functionality with another without either knowing how the other is built inside.
3. **How it works — ask, and receive.** Walk the flow: your app (needs a map on the page) → request → the API (the agreed-upon doorway) → response → the service (Google Maps sends map data back). Your app sends a request through the API; the service sends a response back — and you use the result without ever seeing the other system's code.
4. **Three types.** Web APIs (talk over the internet, e.g. Google Maps API); Operating System APIs (access OS functions — files, network, hardware, e.g. file system access); Library-Based APIs (expose a specific library's functions and resources, e.g. a charting library).
5. **Benefits.** Reuse code (plug in functionality that already exists instead of building from scratch); combine powers (integrate several APIs into one program for more advanced applications); collaborate and innovate (mixing services creates products that wouldn't have been possible alone); better experience (users reach info and features from other apps without leaving yours).
6. **In the wild.** Maps in an app (a website drops in the Google Maps API to show an interactive map); pay without leaving (a social platform uses a payment API so you can buy something inside the app). Prompt students to look around.
7. **Frameworks.** A framework is a set of pre-built software components that give you a foundation for building web applications. Instead of wiring up everything yourself, you start from proven structure and build quickly on top of it.
8. **The lineup.** Introduce React, Angular, Django, Flask, and Ruby on Rails with the wording in Key terms above.
9. **Front vs back.** Sort the lineup: front-end (what users see) — React → JavaScript, components & SPAs; Angular → TypeScript, big front-end apps. Back-end (server side) — Django → Python, full-featured; Flask → Python, minimal; Rails → Ruby, convention-driven. Land the point that there's no single "best."
10. **Recap.** Run through the chips: API, request/response, web APIs, OS APIs, library APIs, reuse code, frameworks, React, Angular, Django, Flask, Ruby on Rails. Restate the big idea.
11. **Homework — "Connect to the wider web."** Assign the checklist (see below).

## Discussion prompts

- **Slide 6:** `// look around` — logins with Google, weather widgets, embedded videos, "share to…" buttons — all APIs.
- **Slide 9:** `// no single "best"` — each framework has strengths & trade-offs. Pick one that fits the project (and the language you know).
- **Slide 10:** `// the big idea` — APIs let your app borrow other apps' powers; frameworks give you a head start so you're not building from zero.

## Watch out for

- **There's no single "best" framework.** Each has strengths and trade-offs — steer students toward picking one that fits the project and the language they know, not toward a "winner."
- **You use the result of an API without ever seeing the other system's code.** Reinforce that the point of an API is to communicate without either side knowing how the other is built inside.

## Homework to assign

Assign "Connect to the wider web" (slide 11):

1. Find a free public API (weather, jokes, dog photos…) and read its docs.
2. Embed one API in your project — a map, a video, or a font service.
3. Skim a framework's homepage — React or Django — and note what it gives you for free.
4. Write two sentences: which framework fits a project you'd like to build, and why?

## Looking ahead

Leave students with the closing line: **stand on the shoulders of giants.** APIs and frameworks let them build on proven work instead of starting from zero — a habit that carries into everything they'll make next.
