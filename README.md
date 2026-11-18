# Jireh Ochygole Samuel · portfolio

A single-file portfolio site. Everything (markup, styles, script) lives in `index.html`, so it
works from a file:// path, GitHub Pages, Vercel, Netlify or any static host with no build step.

## Before you change anything

Open `index.html`, scroll to the bottom, and fill in the two empty strings in `CONFIG`:

```js
var CONFIG = {
  email: "samueljireh752@gmail.com",
  linkedin: "https://www.linkedin.com/in/samuel-jireh-5172b43aa"
};
```

Both are filled in with your real email and LinkedIn. If you ever blank one, its button hides
instead of pointing nowhere. Also check these, which were set from what could be verified:

- `BASED IN` in the hero says **Nigeria · remote**. Change if you prefer a city.
- `CODING SINCE` says **2025**, based on your earliest repos.
- Skills marked *Comfortable* mean you have shipped with them and can debug them alone. Move
  anything you would not defend in an interview down to *Working* or *Learning*.

## Live

Published at **https://jireh7521.github.io** from this repository (`main`, root), served by GitHub
Pages with the free `github.io` HTTPS certificate.

To make a change, edit `index.html` here (or clone the repo and push). Pages redeploys within a
minute. No build step, no Actions workflow.

## What is on the page

- Hero with a live status pill and a terminal card.
- Six project cards, filterable by JavaScript / Python.
- Honest skill levels: Comfortable, Working, Learning, no invented tools.
- How you review AI-generated code.
- A short timeline ending at the current work.
- Dark and light themes (button in the top bar, remembered in `localStorage`).

## Accessibility and performance notes

- One HTML file, no frameworks, no build. About 45 KB before fonts.
- Fonts: Space Grotesk and JetBrains Mono from Google Fonts. Remove the two `<link>` tags to go
  fully offline, and the system font stack takes over.
- Sections are reachable by keyboard, focus rings are visible, and `prefers-reduced-motion` turns
  off the reveal animation and the blinking caret.
