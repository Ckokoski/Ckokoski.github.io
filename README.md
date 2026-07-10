# ckokoski.github.io

Portfolio hub for Christopher Kokoski. Static HTML/CSS/JS, hosted on GitHub Pages.

**Live site:** https://ckokoski.github.io

## Structure

```
index.html                 Main landing page (dark design: hero, stats, disciplines, work, impact, about, contact)
css/portfolio.css          All styling for the landing + instructional design pages
css/fonts.css              @font-face rules for Geist / Geist Mono (files in assets/fonts/)
assets/                    Headshot, favicon, fonts, diagrams
instructional-design/      Instructional design page (light "learning" design)
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
