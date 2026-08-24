# Week 06 Teacher Guide — WordPress

> **Intro to Web Development · ICOM101 / MTEC617 · CalArts · Spring 2026**
> **Week 06 — WordPress**
> _Teacher Guide_

## At a glance

Week 06 is a mostly conceptual week. Students meet WordPress as a content management system (CMS): how it works under the hood, the pieces that make it up, and the everyday tasks of running a site — creating content, choosing a theme, building menus, adding plugins, and keeping everything updated and backed up. There are very few code snippets; the emphasis is on ideas and workflow. This week builds on Weeks 01–05 (HTML and CSS), and the recurring theme is that the HTML and CSS students already know live inside a WordPress theme. The 18-slide lecture ends with a homework checklist on slide 18.

## Learning objectives

By the end of this week, students should be able to:

- Explain what a CMS is and why it removes the need to write HTML and CSS by hand for every page
- Describe how a WordPress page is assembled on each visit
- Name the three pieces — core, themes, plugins — and what each does
- Distinguish Posts from Pages and know when to use each
- Set up a WordPress site locally or on a host, and log into the dashboard
- Create a Post and a Page, build a menu, and install a plugin
- Explain the four hosting types and what to weigh when choosing one
- Understand why to keep WordPress updated and always back up first

## Key terms

- **CMS (content management system)** — lets you create and manage a website through a visual dashboard, with no writing HTML and CSS by hand for every page.
- **PHP** — the language WordPress is built on; the server runs the WordPress code with it.
- **MySQL** — the database that supplies content and settings.
- **Core** — the WordPress engine, the foundation.
- **Themes** — control the layout and design (look and feel); swap one and the whole look changes.
- **Plugins** — add functionality: contact forms, SEO, backups, e-commerce, and thousands more.
- **/wp-admin dashboard** — where everything is managed; you log in by adding /wp-admin to your site's URL, then entering username and password. Left menu: Posts, Pages, Appearance, Plugins, Settings.
- **Posts vs Pages** — Posts are time-based, organized by date, shown in the blog feed and archives, and use categories and tags (news, blog entries, updates). Pages are static content, not dated, not in the blog feed, and use templates for layout (About Us, Contact).
- **Categories & tags** — used to organize Posts.
- **Templates** — used by Pages to control layout, chosen under Page Attributes.
- **Menus** — how visitors navigate the site; built in Appearance ▸ Menus and assigned to a location (header, footer, sidebar).
- **Plugins (as a task)** — searched in the repository, installed, activated, configured, and kept updated; remove ones you don't use.
- **Hosting types** — Shared (many sites share one server; cheapest, simplest; best for beginners/budgets). VPS (your own slice of a server; more control; best for growing traffic). Dedicated (a whole physical server to yourself; priciest, most powerful; best for large, secure sites). Cloud (scale resources up and down on demand; best for spiky traffic).
- **Updates** — bring security patches, bug fixes, and new features; back up first, always.
- **Backups / UpdraftPlus** — a backup plugin like UpdraftPlus saves a full copy of your site (files and database) before you change anything; store off-site and schedule automatic backups.

## Lesson flow

- **S1 — Title.** WordPress. Point out the sign-in address pattern: yoursite.com/wp-admin.
- **S2 — What is WP.** A CMS lets you create and manage a website through a visual dashboard, no writing HTML and CSS by hand for every page. Under the hood it's built on PHP and a MySQL database. It powers everything from simple blogs to complex online stores.
- **S3 — How it works.** A page is assembled on every visit: (1) visitor requests a page in their browser, (2) server + PHP runs the WordPress code, (3) MySQL supplies content and settings, (4) HTML/CSS/JS is generated and sent back to display. Unlike static HTML files, a WordPress page is built fresh from the database each time it's requested.
- **S4 — The pieces.** Core is the WordPress engine (the foundation). Themes control the layout and design — swap one and the whole look changes. Plugins add functionality — contact forms, SEO, backups, e-commerce, and thousands more.
- **S5 — Create a site.** Online (hosted): pick a host (Bluehost, SiteGround…), choose a domain name, follow prompts to install and set username/password, then log in, pick a theme, add content. Locally (your computer): install a local server (XAMPP or MAMP), download WordPress from wordpress.org, create a database, run the installer at localhost/…, then log in and build.
- **S6 — Hosting.** Shared, VPS, Dedicated, Cloud — walk through what each is and who it's best for.
- **S7 — What to weigh.** Cost, Resources (storage/bandwidth/power), Support, Security, Speed.
- **S8 — The dashboard.** Everything is managed from the dashboard (wp-admin). Log in by adding /wp-admin to the site URL, then username and password. Left menu: Posts, Pages, Appearance, Plugins, Settings.
- **S9 — Posts vs Pages.** Posts: time-based, organized by date, in the blog feed and archives, use categories and tags (news, blog entries, updates). Pages: static content, not dated, not in the blog feed, use templates for layout (About Us, Contact).
- **S10 — Creating a post.** Posts ▸ Add New; type a title and write in the visual editor; pick Categories and add Tags; Add Media for images/video; optional featured image (thumbnail) and excerpt (summary); Publish, save draft, or schedule.
- **S11 — Creating a page.** Pages ▸ Add New; add a title and content; choose a Template under Page Attributes to control layout; Add Media; Publish/draft/schedule. Pages are for static content (About, Contact).
- **S12 — Themes.** Using a theme: Appearance ▸ Themes, Live Preview, Activate. Building a theme: needs some HTML, CSS, and PHP; a new folder in wp-content/themes; add style.css (styles) and index.php (main template); use PHP to include header/footer and template tags for dynamic content.
- **S13 — Menus.** Appearance ▸ Menus opens the Menu Editor; name it, Create Menu; Add Items (Pages, Posts, Custom Links); drag and drop to reorder, nest for sub-menus; assign to a location (header, footer, sidebar). Menus are how visitors navigate your site. Different menus in different locations.
- **S14 — Plugins.** Plugins ▸ Add New, search the repository; check description and reviews (well-maintained and compatible?); Install Now then Activate; configure its settings; keep plugins updated, remove ones you don't use.
- **S15 — Updates.** Back up first, always, before any update. Go to the Updates section; Update Now for core (don't close the tab); then update plugins and themes; for major versions check release notes. Updates bring security patches, bug fixes, and new features.
- **S16 — Backups.** A backup plugin like UpdraftPlus saves a full copy of your site — files and database — before you change anything. Install and activate UpdraftPlus; Backup Now before updating; store off-site (Google Drive, Dropbox); schedule automatic backups; Restore if something breaks.
- **S17 — Recap.** Chips: CMS, PHP + MySQL, core/themes/plugins, /wp-admin, posts vs pages, categories & tags, templates, themes, menus, plugins, hosting, updates, backups.
- **S18 — Homework.** "Try WordPress." Walk through the checklist and set expectations for submission.

## Discussion prompts

- On the pieces (S4): "thousands available — free and paid." Ask students what functionality they'd want to add to a site, and let them see how many plugins might exist for it.
- On choosing a host (S7): "also — read reviews, ask for recommendations, and think ahead about scalability and moving hosts later." Prompt students to consider not just today's needs but future growth.
- On themes (S12): "the HTML & CSS you've learned is exactly what lives inside a theme." Connect Weeks 01–05 directly to what's inside a theme.
- On the recap (S17): "the big idea — WordPress manages the site so you can focus on content and design, with the HTML & CSS you know living inside the theme." Use this to tie the whole week together.

## Watch out for

- **Always back up BEFORE any update.** Emphasize the order: back up first, always, before any update.
- **Pages are for static content, not dated like posts.** Students often reach for a Post when they mean a Page. Reinforce that Pages (About, Contact) are static and not organized by date.
- **A WordPress page is built fresh from the database each request, unlike static HTML files.** This is the key mental shift from the static HTML/CSS work of earlier weeks.

## Homework to assign

Assign **"Try WordPress"** (slide 18). Students set up a WordPress site (locally with MAMP/XAMPP or on a free host), install and activate a theme, create one Page (About) and one Post (a blog entry), build a menu and add their pages to it, install one plugin, and make a backup. See `assignment.md` for the full write-up and grading.

## Looking ahead

The through-line to carry forward: content first, code underneath. Students have seen that the HTML and CSS they know lives inside a theme, and that WordPress manages the site so they can focus on content and design.
