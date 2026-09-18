# Camp SnickerWillow Hollow — free chapters site

A single static page: cover, blurb, an embedded/downloadable PDF of the first
four chapters, and a link to buy the full book.

## Files

- `index.html` — the whole site
- `assets/cover.jpg` — book cover (web-optimized)
- `assets/first-four-chapters.pdf` — the free excerpt

## Put it on GitHub Pages

1. Create a new repository on GitHub (e.g. `camp-snickerwillow-hollow`).
2. Copy `index.html` and the `assets/` folder into the repo (keep that folder
   name and structure — the page links to `assets/...`).
3. Commit and push:
   ```
   git init
   git add .
   git commit -m "Add free chapters site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
4. On GitHub: **Settings → Pages → Build and deployment → Source** → select
   `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. GitHub gives you a live URL in a minute or two, usually
   `https://<your-username>.github.io/<repo-name>/`.

## Notes

- The PDF preview uses an `<embed>` tag. Most desktop browsers show it inline;
  a few mobile browsers won't, which is why there's always a visible
  "Download the PDF" button as a fallback.
- The Amazon link is already wired to `https://a.co/d/0a4B5YZD` in two spots
  (top button and footer) — update both if the link ever changes.
- Everything is plain HTML/CSS, no build step, so you can just keep editing
  `index.html` directly.
