# Dr. Smith Mehta — Academic Website

A static, multi-page personal academic website for Dr. Smith Mehta,
Assistant Professor in the Centre for Media & Journalism Studies,
University of Groningen.

## Pages
- `index.html` — Home (bio, expertise, featured books & publications)
- `research.html` — Research, full publication list (with filters), grants, talks
- `teaching.html` — Teaching, courses, thesis supervision
- `cv.html` — Full curriculum vitae
- `contact.html` — Contact details & links

## Structure
```
index.html, research.html, teaching.html, cv.html, contact.html
style.css        # shared design system (all styling)
site.js          # mobile nav + scroll reveal
assets/
  smith-mehta.jpg
```

No build step and no dependencies — just static HTML/CSS/JS.
Fonts (Instrument Serif, Hanken Grotesk, Space Mono) load from Google Fonts.

## Run locally
Open `index.html` in a browser, or serve the folder:
```
python3 -m http.server
```
then visit http://localhost:8000

## Deploy with GitHub Pages
1. Create a new repository and upload these files to the root.
2. In **Settings → Pages**, set **Source** to the `main` branch, `/ (root)` folder.
3. Your site goes live at `https://<username>.github.io/<repo>/`.

## To update
- **Google Scholar / ORCID links** — replace the placeholder URLs in the
  footer (and on `contact.html`) with the real profile URLs.
- **Publications** — add a new `<article class="pub" data-cat="article">…</article>`
  block in `research.html` (categories: `article`, `chapter`, `progress`).
- **Photo** — replace `assets/smith-mehta.jpg` (square works best).

© 2026 Dr. Smith Mehta
