# Rohans Junior School — Responsive Website Prototype

A small, connected website for **Rohans Junior School**, located in
Sembabule District, Uganda. Built as part of a Semantic HTML and
Responsive Interfaces assignment.

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
- Visible focus outlines are shown for keyboard users.

## Responsive Design (CSS)

Styling is in an external stylesheet (`style.css`), linked from all pages.
The approach is **mobile-first**:

- Default styles target small screens: header and navigation stack vertically.
- From **700px and up**, a media query switches the header to a grid layout
  with the logo on the left and navigation on the right, and places content
  cards side by side using CSS Grid.
- **Flexbox** is used for the navigation list, form fields, and footer.
- Images use `max-width: 100%` so they never overflow their container.
- Colour contrast and keyboard focus visibility meet accessibility guidance.

## Testing

Tested at **390px** (mobile) and **1366px** (desktop) using Chrome DevTools.

**Problem found and fixed:** The school logo was not displaying on the Home
page because the filename in the HTML did not match the file in the `images`
folder. The reference was corrected and the logo now displays correctly at
both screen sizes.

## Author

AMANYA AARON — Sembabule District, Uganda
