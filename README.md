# The Line — FreeAPI Meals Listing Interface

A meals/recipes browser built for the **FreeAPI: Meals Listing Interface** project (Web Dev Cohort 2026), themed like a kitchen order rail — each meal is a torn ticket you pull to read the full recipe.

**API used:** `https://api.freeapi.app/api/v1/public/meals`

## Features

- Fetches all meals from the paginated API (30 pages) in the background with a live progress indicator
- Full-text search across dish name, cuisine, category, and ingredients
- Filter by **category** ("station") and **cuisine/area** ("flag")
- Sort by name (A–Z / Z–A) or ingredient count
- Client-side pagination (12 tickets per page) with numbered pager
- Click any ticket to open a detail view: full ingredient list with measures, numbered method steps, tags, source link, and YouTube link (when available)
- Responsive layout, keyboard-accessible cards (Enter to open, Esc to close modal), lazy-loaded images

## Tech

Plain HTML, vanilla JavaScript (no build step), and Tailwind CSS via CDN. Single file: `index.html`.

## Run locally

No build tools required — just open `index.html` in a browser, or serve it:

```bash
npx serve .


Then visit `http://127.0.0.1:5500/index.html` 

## Deployment

**GitHub Pages**
1. Push this repo to GitHub.
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
3. Your live link will be `https://<username>.github.io/<repo-name>/`.


**Vercel**
1. Import the GitHub repo at [vercel.com/new](https://vercel.com/new).
2. Framework preset: "Other" — no build command, output directory `.`.

## Project structure

```
.
├── index.html   # everything: markup, styles, and app logic
└── README.md
└── Image  #food-background
```
