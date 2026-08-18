# ckokoski.github.io

Portfolio hub for Christopher Kokoski. Static HTML/CSS/JS, hosted on GitHub Pages.

**Live site:** https://ckokoski.github.io

## Structure

```
index.html                 Main landing page (dark design: hero, stats, disciplines, work, impact, about, contact)
css/portfolio.css          All styling for the landing + instructional design pages
css/fonts.css              @font-face rules for Geist / Geist Mono (files in assets/fonts/)
assets/                    Headshot, favicon, fonts, diagrams
builds/                    Build Lab hub + one folder per tool case study
instructional-design/      AI Training & Learning Design page (light "learning" design)
  files/                   Standards PDFs and course design documents
ai-enablement/             AI enablement lane page + pdfs/
technical-writing/         Technical writing samples
data-analytics/            Data & analytics lane page
courses/                   Self-contained interactive course builds
style.css                  Legacy shared styling for the lane pages (do not delete)
```

## Local preview

```bash
python -m http.server 4178 --directory .
# then open http://localhost:4178
```

## Updating stats and projects

- Hero stats and the Impact section live in `index.html` (look for the `Stats:` and
  `Impact:` HTML comments). Only use approved, verifiable numbers.
- Selected-work cards are in the `work-grid` div in `index.html`. Each card needs a
  `data-type` matching one of the filter buttons.
- Instructional design samples are the six cards in
  `instructional-design/index.html` under `learning-projects`. Cards 03 and 04 are
  anchor links to the project-brief section further down the page; swap the `href`
  to a course URL when those builds ship.

## Adding a new build

1. Create `builds/<slug>/index.html` by copying `builds/tablegrab/index.html`
   (or `builds/speed-to-lead/index.html` for a video-led case study) and editing
   the copy. Drop the tool's assets (screenshots, video, zip, hostable HTML)
   into the same folder.
2. Add a card to the grid in `builds/index.html` at the `ADD NEW BUILDS HERE`
   comment. Set `data-type` to one or more of the filter values
   (pipe-separated, e.g. `data-type="API|MCP"`), and keep the `work-index`
   numbers sequential.
3. Optionally add a card to the Selected Work grid in the root `index.html`
   (`data-type="Builds"`, `href="builds/"`).
4. Preview locally, then commit and push to `main` to deploy.
