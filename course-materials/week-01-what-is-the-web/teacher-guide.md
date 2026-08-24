# Week 01 Teacher Guide — What is the Web?

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 01 — What is the Web?**
> _Teacher Guide_

## At a glance

- **Week:** 01 of 9
- **Topic:** What is the Web?
- **Deck:** ~13 slides
- **Session:** First class — no prerequisite.
- **What students leave with:** A mental model of the web (server/client, front/back end), a short history of HTML and CSS, the difference between markup and scripting, an understanding of what happens when you visit a website, the three kinds of server response, and the homework of reading three sites "like a designer."

## Learning objectives

By the end of this session, students should be able to:

- Explain what a server and a client are, and that all the code we write runs on the client.
- Connect front end / back end to client side / server side.
- Name who proposed HTML and CSS, and when and where.
- Distinguish a markup language from a scripting language.
- Describe the four steps of visiting a website, and the role of IP addresses and DNS.
- Identify the three kinds of server response and which one we build (a static site).

## Key terms

server
: The computer that hosts your website. Servers make the internet work — in this class we'll avoid dealing with them directly wherever possible.

client
: The computer visiting your website (the opposite of the server). All the code we write runs on the client.

front / back end
: Client side / server side, respectively. e.g. "HTML is a front-end language."

markup
: Prepares the structure and look of a page — presentational. No logic, no algorithms, asks the computer nothing. Tells the browser how to structure & style data. e.g. HTML, CSS, XML.

scripting
: Gives instructions to control another program — doesn't work standalone. Interpreted, not compiled — scanned line by line. No compiler involved. e.g. JavaScript, PHP, Perl, Python, VBScript.

IP address
: Every site has a unique IP address — like a phone number.

DNS
: The address book that maps names to addresses. (Domain Name Server.)

## Lesson flow

**Slide 1 — Title.** Introduce the course: "Intro to Web Development," Week 01. Set the tone for the first class.

**Slide 2 — Directories, not destinations.** Cover the framing for how we'll build: we build sites that act as a hub for content — but don't always host the content themselves. Talking point: for now we're less interested in fully-featured, rich-media browsing portfolios, and more concerned with creating useful directories that link to content around the web.

**Slide 3 — Key terms (server / client / front & back end).** Introduce the three core terms using the definitions above. Emphasize that all the code we write runs on the client, and that we'll avoid dealing with servers directly wherever possible.

**Slide 4 — Belonging.** "Everyone is welcome in this class. We all belong here." Talking point: coding is not reserved for a particular type of person. It's a skill that constantly evolves — and anyone interested in learning it can benefit, and master it, regardless of age, gender, or background. It's an inclusive, accessible field. Worth saying out loud on day one.

**Slide 5 — Why (HTML & CSS are the front door).** They're essential for anyone building websites or web apps — and a solid grasp of both makes it far easier to pick up JavaScript, which adds interactivity and dynamic behavior. Talking point: they're also relatively simple to learn, which makes them a great first step into programming.

**Slide 6 — Skills (whole-course map).** Show the chips: HTML, CSS, JavaScript, jQuery, Command Line, Linux, GitHub, WordPress, APIs, Software Best Practices, Reverse Engineering. Discussion prompt (// discuss): we don't learn these all at once. Today is just the first two chips (HTML & CSS).

**Slide 7 — HTML history.** "HyperText Markup Language." Proposed by Tim Berners-Lee; year 1989; at CERN, Switzerland; why: to share scientific information between researchers at different institutions — structuring & formatting it for the World Wide Web. Discussion prompts (// discuss): old computers — green-on-black screens, SGML → government funding for the internet & institutions → markup language vs programming language.

**Slide 8 — CSS history.** "Cascading Style Sheets." Proposed by Håkon Wium Lie; year 1994, also at CERN; CSS1 released 1996 — basic font & color control. The idea: separate a site's presentation from its structure (which HTML defines). Talking point: CSS became the tool for building visually consistent, appealing sites — and today it's supported by every modern browser.

**Slide 9 — Scripting vs markup.** Draw the contrast clearly. Scripting: gives instructions to control another program — doesn't work standalone. Interpreted, not compiled — scanned line by line. No compiler involved. e.g. JavaScript, PHP, Perl, Python, VBScript. Markup: prepares the structure and look of a page — presentational. No logic, no algorithms, asks the computer nothing. Tells the browser how to structure & style data. e.g. HTML, CSS, XML. Footnote to stress: all scripting languages are programming languages — but not all programming languages are scripting languages.

**Slide 10 — Visiting a website.** "Like calling a phone number." Every site has a unique IP address — like a phone number. DNS is the address book that maps names to addresses. Walk the four steps: (1) You type an address into the browser and hit enter. (2) Your ISP asks a DNS (Domain Name Server) where that site lives. (3) The DNS resolves the request — it looks up the domain and returns the site's IP address to your ISP, which forwards your request there. (4) The server receives your request and is expected to generate a response.

**Slide 11 — The response.** "Three ways to answer." A Twitter server → dynamically generates your custom homepage and returns it. An API endpoint → calculates some data and returns it in a machine-readable format. A static site → just returns a pre-written chunk of HTML. Emphasize: the static site is what we're doing.

**Slide 12 — Homework.** "Read the web like a designer." Assign the three-site exploration (see below and assignment.md). Walk through the checklist so students know what to look for.

**Slide 13 — Closing.** "Next week, we write our first tags." Up next: hand-writing HTML — the anatomy of an element.

## Discussion prompts

- (Slide 6) We don't learn these all at once. Today is just the first two chips (HTML & CSS).
- (Slide 7) Old computers — green-on-black screens, SGML.
- (Slide 7) Government funding for the internet & institutions.
- (Slide 7) Markup language vs programming language.

## Watch out for

- **Markup vs programming/scripting language.** This is the big one for slide 9. Students often assume anything that looks like code is "programming." Reinforce that markup prepares structure and look, has no logic or algorithms, and asks the computer nothing — while scripting gives instructions to control another program and is interpreted line by line.
- **The scripting/programming relationship.** Say it plainly: all scripting languages are programming languages — but not all programming languages are scripting languages.
- **Server vs client confusion.** Keep reinforcing that the client is the computer visiting the site (the opposite of the server), and that all the code we write runs on the client.

## Homework to assign

Assign "Read the web like a designer" (full details in **assignment.md**). In short: students choose three websites (businesses, organizations, or personal blogs), spend at least 5 minutes on each noting what they like and dislike, and write a short summary analyzing those elements and why, with specific examples. They should use the exploration checklist (overall design, navigation, content organization, interactive elements, responsiveness).

## Looking ahead

"Next week, we write our first tags." Up next: hand-writing HTML — the anatomy of an element.
