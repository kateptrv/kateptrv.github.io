# Personal website

Static site for [kateptrv.github.io](https://kateptrv.github.io). Plain HTML + CSS, no build step.

## Files

- `index.html` — About / homepage
- `publications.html` — Full publication list
- `teaching.html` — Teaching experience and mentored theses
- `cv.html` — CV
- `styles.css` — Shared styling
- `profile.jpg` - Headshot
- `cv.pdf` — CV pdfg

## Placeholders to fill in

Search for these in the files and update before publishing:

- `YOUR_ID` in `index.html` — your Google Scholar profile ID
- `github.com/kateptrv` in `index.html` — confirm or change GitHub username
- `https://osf.io/` in `index.html` — your OSF profile URL (or remove the link)
- The `<!-- Replace with: <img ... -->` block in `index.html` — swap the "photo"
  placeholder for `<img src="profile.jpg" alt="Kate Petrova">`

## Deploying to GitHub Pages

GitHub Pages serves user sites from a repo named `<username>.github.io`.

```bash
cd /Users/katepetrova/website
git init
git add .
git commit -m "Initial site"
git branch -M main
# create an empty repo named exactly kateptrv.github.io on github.com first,
# then:
git remote add origin https://github.com/kateptrv/kateptrv.github.io.git
git push -u origin main
```

Within a minute or two the site will be live at <https://kateptrv.github.io>.

To preview locally, just open `index.html` in a browser, or run:

```bash
cd /Users/katepetrova/website
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing

Each page is a small, self-contained HTML file. Update the content directly —
no templates or build tools involved. The shared header/footer is duplicated
across pages; if you add a new section to the nav, update it in all four files.
