# Agent Reference — Roadmap File Structure

_This file is for the agent's own consistency reference, not for users to copy or edit.
When creating a new roadmap file, use this as the structural baseline and adapt as needed._

---

## File header

```markdown
# Roadmap — [Period or Theme]

[One-paragraph overview: what this covers and what success looks like.]
```

---

## Active item block

```markdown
### [Item Title]

- **Status:** discovery / planned / in progress / shipped / paused / cancelled
- **Owner:** [Person or squad]
- **Quarter:** [e.g. Q1 2026]
- **Priority:** P1 / P2 / P3
- **Tags:** [free-form, comma-separated]
- **Depends on:** [Other item, if any]

**What:** What is being built or changed.

**Why:** The problem it solves or opportunity it captures.

**Success looks like:** How we'll know it's done and working.

**Notes:** Known risks, open questions, or blockers. Omit if none.
```

---

## Shipped table

```markdown
## Shipped This Period

| Item | Owner | Shipped |
|------|-------|---------|
| Item name | Squad | YYYY-MM-DD |
```

---

## On hold / cancelled table

```markdown
## On Hold / Cancelled

| Item | Reason | Owner |
|------|--------|-------|
| Item name | Reason | Squad |
```

---

## Consistency rules

- Use the same status vocabulary throughout a file
- `Notes:` section is optional — omit rather than leaving it blank
- Items should be roughly equal in depth — if one has a `Why`, all should
- Shipped and On Hold tables use ISO dates (YYYY-MM-DD)
- New files go in `roadmap/` with kebab-case names: `q1-2026.md`, `platform.md`
