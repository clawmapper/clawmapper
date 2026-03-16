# Template: Board Slide

**Use this template by saying something like:**
> "Make me a board slide for Q1" or "Generate a board update covering key projects this quarter"

---

## Agent Instructions

When using this template, produce a **self-contained HTML file** written to
`outputs/YYYY-MM/board-slide-[period].html`.

### Audience
Board of directors or senior leadership. They want:
- Outcomes and progress, not activity
- Honest status — don't oversell
- What's on track, what's at risk, and why it matters commercially

### Structure to follow

1. **Title slide** — Period, date, company name
2. **Headline** — One sentence: what's the story this quarter?
3. **Key initiatives** — 3–5 items maximum. For each:
   - Name and one-line description
   - Status indicator (on track / at risk / shipped)
   - Key metric or outcome (not tasks completed)
4. **Wins** — 2–3 things shipped or achieved worth celebrating
5. **Risks & watch items** — 1–3 honest flags with mitigations
6. **Looking ahead** — What does next quarter set up?

### HTML style guidance

- Clean, minimal design — dark background (`#0f172a`), white text (`#f8fafc`)
- Large, readable fonts — minimum 18px body, 32px headings
- Status colours: on track = `#22c55e`, at risk = `#f59e0b`, shipped = `#3b82f6`, cancelled/paused = `#6b7280`
- No external dependencies — all CSS inline or in a `<style>` block
- Single scrollable page or use `<section>` blocks for visual separation
- Include generation date and source files in an HTML comment at the top

### What to read first

1. The roadmap file(s) for the relevant period
2. `context/strategy.md` — to frame items against OKRs
3. `memory/MEMORY.md` — for any standing board context
