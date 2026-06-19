# ckokoski.github.io

Portfolio hub for Christopher Kokoski. One site, organizing work samples across three areas:

- **Instructional Design & Learning** — evidence-based learning design and course builds (Rise 360, Articulate Storyline).
- **AI Enablement** — adoption playbook, prompt cookbook, a workflow case study, and a responsible-use framework.
- **Data & Analytics** — hosted in a separate repository: [data-analytics-portfolio](https://github.com/Ckokoski/data-analytics-portfolio).

**Live site:** https://ckokoski.github.io

## Structure

```
index.html                 Routing homepage with three lane cards
style.css                  Shared styling
instructional-design/      Instructional design lane page
ai-enablement/             AI enablement lane page
  pdfs/                    AI enablement work samples (PDF)
assets/                    Favicon and supporting diagrams
```

## Local preview

```bash
python -m http.server 4178 --directory .
# then open http://localhost:4178
```

## Updating project links

Placeholder cards on the lane pages are marked **Coming soon**. Each has an HTML
comment above it showing the exact swap instructions and token (for example
`[RISE_COURSE_LINK_TO_COME]` or `[LINK_TO_COME]`). To publish a link, replace the
placeholder `<article class="card card--soon">` block with an `<a class="card" href="...">`
as described in the comment.
