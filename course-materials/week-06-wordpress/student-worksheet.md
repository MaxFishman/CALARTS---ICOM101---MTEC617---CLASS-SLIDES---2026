# Week 06 Worksheet — WordPress

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 06 — WordPress**
> _Student Worksheet_

Work through the exercises below to review what WordPress is, how it builds a page, and the everyday tasks of running a site. Check your work against the answer key at the end.

## Key terms

Match each term to its description.

**Terms:** CMS · core · themes · plugins · /wp-admin · categories · templates

1. _____ The WordPress engine — the foundation.
2. _____ Control the layout and design (look and feel); swap one and the whole look changes.
3. _____ Add functionality — contact forms, SEO, backups, e-commerce, and thousands more.
4. _____ Lets you create and manage a website through a visual dashboard, with no writing HTML and CSS by hand for every page.
5. _____ Add this to your site's URL to log into the dashboard.
6. _____ Used to organize Posts (along with tags).
7. _____ Used by Pages to control layout, chosen under Page Attributes.

## Posts vs Pages

Sort each example into the right column — is it a **Post** or a **Page**? Then, for each, note whether it is **dated** or **static**.

**Examples:** News · About Us · Blog entries · Contact · Updates

| Example | Post or Page? | Dated or Static? |
| --- | --- | --- |
| News | | |
| About Us | | |
| Blog entries | | |
| Contact | | |
| Updates | | |

## The request flow

Put these four steps in the correct order to show how a WordPress page gets built on every visit. Number them 1–4.

- _____ MySQL supplies content and settings
- _____ HTML/CSS/JS is generated and sent back to display
- _____ Visitor requests a page in their browser
- _____ Server + PHP runs the WordPress code

## Short answer

1. What two technologies is WordPress built on under the hood?

2. How do you log into the dashboard?

3. What do **themes** control, versus what do **plugins** control?

4. Name the four hosting types.

5. Why should you keep WordPress updated?

6. What does a backup plugin like UpdraftPlus do?

## Try it

A mini version of the homework. Complete these three tasks and jot a note next to each when it's done:

1. **Spin up a site** — set up a WordPress site locally (MAMP/XAMPP) or on a free host.
2. **Activate a theme** — install and activate a theme you like.
3. **Make one Page and one Post** — create one Page (About) and one Post (a blog entry).

## Answer key

**Key terms**

1. core
2. themes
3. plugins
4. CMS
5. /wp-admin
6. categories
7. templates

**Posts vs Pages**

| Example | Post or Page? | Dated or Static? |
| --- | --- | --- |
| News | Post | Dated |
| About Us | Page | Static |
| Blog entries | Post | Dated |
| Contact | Page | Static |
| Updates | Post | Dated |

Posts are time-based and organized by date; Pages are static content, not dated.

**The request flow**

1. Visitor requests a page in their browser
2. Server + PHP runs the WordPress code
3. MySQL supplies content and settings
4. HTML/CSS/JS is generated and sent back to display

Unlike static HTML files, a WordPress page is built fresh from the database each time it's requested.

**Short answer**

1. PHP and a MySQL database.
2. Add /wp-admin to your site's URL (for example, www.example.com/wp-admin), then enter your username and password.
3. Themes control the layout and design (the look and feel) — swap one and the whole look changes. Plugins add functionality — contact forms, SEO, backups, e-commerce, and thousands more.
4. Shared, VPS, Dedicated, and Cloud.
5. Updates bring security patches, bug fixes, and new features. (And always back up first, before any update.)
6. It saves a full copy of your site — files and database — before you change anything, can store it off-site, can run on a schedule, and can restore your site if something breaks.
