# Jireh Ochygole Samuel · portfolio

A single-file portfolio site. Everything (markup, styles, script) lives in `index.html`, so it
works from a file:// path, GitHub Pages, Vercel, Netlify or any static host with no build step.

## Before you publish

Open `index.html`, scroll to the bottom, and fill in the two empty strings in `CONFIG`:

```js
var CONFIG = {
  email: "",       // e.g. "samuel@example.com"
  linkedin: ""     // e.g. "https://linkedin.com/in/samuel-jireh"
};
```

Both buttons stay hidden until a value is set, so there is nothing fake on the page while you
decide. Also check these, which I set from what I could verify:

- `BASED IN` in the hero says **Nigeria · remote**. Change if you prefer a city.
- `CODING SINCE` says **2025**, based on your earliest repos.
- Skills marked *Comfortable* mean you have shipped with them and can debug them alone. Move
  anything you would not defend in an interview down to *Working* or *Learning*.

## Publish it free on GitHub Pages

1. Create a repository named `Jireh7521.github.io` (your username, exactly).
2. From this folder:

```bash
git init
git add index.html README.md
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/Jireh7521/Jireh7521.github.io.git
git push -u origin main
```

3. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Live at https://jireh7521.github.io within a minute or two.

Prefer a project repo instead, like `portfolio`? Pages then serves it at
`https://jireh7521.github.io/portfolio/`. The page uses hash anchors only, so no base-path
configuration is needed either way.

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
