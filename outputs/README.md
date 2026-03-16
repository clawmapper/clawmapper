# Outputs

Generated artifacts live here. The agent writes to this folder when asked to
produce slides, summaries, reports, or other stakeholder-facing content.

---

## Naming Convention

```
outputs/YYYY-MM/slug-description.ext
```

Examples:
```
outputs/2026-03/board-slide-q1-overview.html
outputs/2026-03/stakeholder-update-march.md
outputs/2026-03/growth-squad-sprint-summary.pdf
```

- `YYYY-MM` is the month the artifact was generated (not the period it covers)
- The slug should be descriptive enough that someone browsing the folder knows
  what they're looking at without opening the file
- Never overwrite an existing output — the agent creates a new file if an update
  is needed (e.g. `board-slide-q1-overview-v2.html`)

---

## Formats

| Format | Use case |
|--------|----------|
| `.html` | Slides, visual summaries, stakeholder dashboards — self-contained, no CDN deps |
| `.md`   | Written updates, email drafts, sprint summaries |
| `.pdf`  | Formal reports, documents intended for print or download |
| `.pptx` | When a PowerPoint deck is specifically requested |

---

## Viewing HTML Outputs

HTML files are self-contained. Open them directly in a browser. If the repo has
GitHub Pages enabled, outputs can be served publicly from this folder.
