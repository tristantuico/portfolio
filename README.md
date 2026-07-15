# Tristan Tuico — QA Automation Portfolio

A single-page portfolio site, styled around a test-report aesthetic (pytest-inspired hero, skills as "modules", projects as "test suites").

## Files
- `index.html` — the whole site (HTML + CSS + a little JS-free interactivity). No build step needed.

## Before you publish — edit these
1. **Hero assertions** — near the top of `index.html`, tweak the checklist under your name.
2. **Projects** — two sample projects are included (API regression suite, Robot Framework UI suite). Replace names, descriptions, metrics, and the `#` links with your real repo URLs.
3. **Experience timeline** — fill in real roles/dates.
4. **Contact links** — update the `mailto:`, GitHub, and LinkedIn links in the footer.
5. **Resume button** — the "download resume" button currently points to `#`. Either link it to a PDF you upload to the repo (e.g. `resume.pdf`) or remove it.

## How to publish on GitHub Pages

1. Create a new GitHub repo (e.g. `tristan-portfolio`).
2. Upload `index.html` (and `resume.pdf` if you add one) to the repo — either via the GitHub web UI ("Add file → Upload files") or:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/tristan-portfolio.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
5. Save. GitHub will give you a live URL, usually:
   `https://<your-username>.github.io/tristan-portfolio/`
   (takes 1–2 minutes to go live after first deploy)

That's it — no build tools, no dependencies, just static HTML.
