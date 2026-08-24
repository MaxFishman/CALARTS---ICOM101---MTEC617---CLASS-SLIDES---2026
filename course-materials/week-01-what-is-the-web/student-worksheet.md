# Week 01 Worksheet — What is the Web?

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 01 — What is the Web?**
> _Student Worksheet_

Everything here can be answered from this week's lecture.

## Key terms

For each definition, name the term. (For the last two, we give you the term — write the definition in your own words.)

1. The computer that hosts your website. → **______________**
2. The computer visiting your website (the opposite of the server). → **______________**
3. Client side. (As in, "HTML is a ______-end language.") → **______________**
4. Server side. → **______________**
5. The address book that maps names to addresses. → **______________**
6. Every site has a unique one of these — like a phone number. → **______________**
7. **scripting** → ______________________________________________
8. **markup** → ______________________________________________

## Understand the flow

**A. Put the four steps of visiting a website in order (1–4).**

- ___ The DNS resolves the request — it looks up the domain and returns the site's IP address to your ISP, which forwards your request there.
- ___ You type an address into the browser and hit enter.
- ___ The server receives your request and is expected to generate a response.
- ___ Your ISP asks a DNS (Domain Name Server) where that site lives.

**B. Name the three kinds of server response** ("three ways to answer"), and give the one-line description of each.

1. ______________ → ______________________________________________
2. ______________ → ______________________________________________
3. ______________ → ______________________________________________

## Short answer

1. Who proposed HTML, and in what year? Where were they working?
2. Who proposed CSS, and in what year?
3. CSS separates a site's ______________ from its ______________ (which HTML defines).
4. Which of the three response types is the one "we're doing" in this class?
5. Complete the rule: all scripting languages are ______________ languages — but not all ______________ languages are ______________ languages.

## Try it

A short version of this week's homework. Pick **one** website — a business, an organization, or a personal blog — and spend a few minutes on it. Then answer using the exploration checklist:

- What's the overall design? Is it visually appealing?
- Is the navigation intuitive — can you find things easily?
- Is the content organized in a logical way?
- Any interactive elements — forms, videos, games?
- Is it responsive to the size of the screen?

Write two or three sentences on what you liked or disliked, with a specific example.

---

## Answer key

**Key terms**

1. server
2. client
3. front (front-end)
4. back end
5. DNS (Domain Name Server)
6. IP address
7. scripting — Gives instructions to control another program; doesn't work standalone. Interpreted, not compiled — scanned line by line. No compiler involved. e.g. JavaScript, PHP, Perl, Python, VBScript.
8. markup — Prepares the structure and look of a page; presentational. No logic, no algorithms, asks the computer nothing. Tells the browser how to structure & style data. e.g. HTML, CSS, XML.

**Understand the flow**

A. Order: 1) You type an address into the browser and hit enter. 2) Your ISP asks a DNS (Domain Name Server) where that site lives. 3) The DNS resolves the request — it looks up the domain and returns the site's IP address to your ISP, which forwards your request there. 4) The server receives your request and is expected to generate a response.

B. The three responses:
- A Twitter server → Dynamically generates your custom homepage and returns it.
- An API endpoint → Calculates some data and returns it in a machine-readable format.
- A static site → Just returns a pre-written chunk of HTML. (This is what we're doing.)

**Short answer**

1. Tim Berners-Lee, in 1989, at CERN, Switzerland.
2. Håkon Wium Lie, in 1994. (CSS1 released 1996.)
3. presentation; structure
4. A static site.
5. programming; programming; scripting.
