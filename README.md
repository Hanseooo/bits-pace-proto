# PACE × BITS — Student Tech Organization Brand Exploration

A lightweight, responsive, **static website** for sharing two proposed visual identities with founding members. No framework, npm install, backend, API keys, or build command required.

## Pages

| Route | Purpose |
|---|---|
| `/` | Side-by-side **brand comparison**, including interactive workshop/hackathon/talk posters and links to complete identity directions. |
| `/pace/` | Full **PACE** (Programmers' Association for Computing Excellence) brand direction: academic progress, milestone path, palettes, typography, identity studies, and event/merch concepts. |
| `/bits/` | Full **BITS** (Builders in Technology and Software) brand direction from the supplied HTML: pixel B, builder culture, events, merch, and the original **green / blue / red theme switcher**. |

The original BITS layout, design tokens, and interactive event/theme controls are preserved. Only a small cross-page navigation bar has been added. The PACE direction uses the PACE design language developed in the comparison.

## Deploy to GitHub + Vercel

1. Create a new repository on GitHub, e.g. `pace-bits-brand-study`.
2. Upload the **contents of this folder** to the repository root, keeping `index.html`, `pace/index.html`, and `bits/index.html` in their current relative locations.
3. In [Vercel](https://vercel.com/new), choose **Add New → Project**, import the repository, and deploy with **Framework Preset: Other**, **Root Directory: `./`**, **Build Command: none**, and **Output Directory: `./`** (or leave these empty/default for a plain static site, when Vercel accepts that).
4. Share the generated Vercel URL. The comparison will load at the root, and the brand prototypes at `/pace/` and `/bits/`.

You can also preview locally by opening `index.html` directly in a browser. For a local server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000/`, `http://localhost:8000/pace/`, and `http://localhost:8000/bits/`.

## Editing guide

- Comparison copy and style: `index.html`
- PACE copy, colors, and applications: `pace/index.html`
- BITS copy, color themes, and applications: `bits/index.html`
- All CSS and JavaScript are embedded in their respective HTML pages. Shared navigation uses relative URLs, so the site also works from a nested static-hosting path.
- BITS theme selection persists on the member's own browser using `localStorage`; it does not sync across visitors.

## Scope

This is a **conceptual brand exploration**, not an official school identity or operating organization website. Logos, events, mockups, and slogans are design studies. Check name/logo availability and obtain school approval before adopting an identity officially. No tracking, voting system, or data collection is included.

Google Fonts (Space Grotesk and DM Mono) load from Google's CDN when online; system fallback fonts render when offline.
