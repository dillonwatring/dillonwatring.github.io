# Personal site

A static site for Dillon Watring — bio, current role, publications, blog, and fiction. No build step; plain HTML/CSS.

## Files

- `index.html` — homepage (about, role, links, publications pointer)
- `blog.html` — blog post list (placeholder until first post)
- `fiction.html` — fiction list (placeholder until first story)
- `assets/style.css` — shared styles (light/dark mode aware)

## Before you publish

Username placeholders have been filled in with `dillonwatring` throughout `index.html`.

Also edit the "About" paragraph in `index.html` — it's a placeholder bio, replace with your own words.

## Publish with GitHub Pages

1. Create a GitHub account if you don't have one: https://github.com/signup
2. Create a new **public** repository named exactly `dillonwatring.github.io` (replace with your username). This exact naming is what makes GitHub Pages serve it at the root domain automatically.
3. Push this folder's contents to that repo:
   ```
   cd personal-site
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/dillonwatring/dillonwatring.github.io.git
   git push -u origin main
   ```
4. In the repo's Settings → Pages, confirm the source is set to the `main` branch (usually auto-detected for this repo naming pattern).
5. Your site will be live at `https://dillonwatring.github.io/` within a few minutes.

## Adding blog posts / stories

Simplest approach for now: duplicate a page (e.g. `blog.html`) into a new file per post, and add a `<div class="card">` link to it from `blog.html`/`fiction.html` (there's a commented example in each file). If you end up writing frequently, GitHub Pages also supports Jekyll natively (Markdown posts, no manual HTML) — worth switching to once you have more than a few posts.

## Note on Google Knowledge Panels

Worth calibrating expectations: a personal website is a useful *supporting* signal (it gives Google a canonical page with structured data — the `Person` JSON-LD already included here — and a place to link your Scholar/LinkedIn profiles together), but Knowledge Panels are generated when Google's systems judge someone/something "notable" enough to have an entity — this usually comes from independent coverage (news, institutional pages, Wikipedia/Wikidata), not from a self-published site alone. This site is a good foundation piece, not a guaranteed trigger by itself.
