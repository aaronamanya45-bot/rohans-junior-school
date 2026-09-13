# Rohans Junior School — Semantic HTML Prototype

A small, connected website prototype for **Rohans Junior School**, located in
Sembabule District, Uganda. Built as part of a Semantic HTML assignment.

## Pages

- **Home** (`index.html`) — welcome message, school highlights, quick notice.
- **About** (`about.html`) — school story, mission and values, classes offered.
- **Contact** (`contact.html`) — contact details and an enquiry form.

## Navigation

A navigation menu appears in the `<header>` of every page and links to all
three pages. The current page is marked with `aria-current="page"`.

## Semantic HTML Elements Used

- `<header>` — page banner
- `<nav>` — main navigation
- `<main>` — primary content of each page
- `<section>` — grouped related content
- `<article>` — individual highlights and value items
- `<aside>` — supplementary notices
- `<figure>` / `<figcaption>` — images with captions
- `<address>` — contact details
- `<footer>` — copyright and secondary links

## Form

The Contact page contains a form that collects:

- Full name
- Email address
- Phone number
- Subject (dropdown)
- Message

## Accessibility Decisions
- Every image has descriptive `alt` text.
- Every form input has a `<label>` linked via the `for` attribute matching
  the input's `id`.
- Headings follow a logical order (`<h1>`, then `<h2>`, then `<h3>`).
- Link text is descriptive rather than "click here".
- `<nav>` is labelled with `aria-label`, and `aria-current="page"` marks the
  current page for screen reader users.

## Author

AMANYA AARON— Sembabule District, Uganda
