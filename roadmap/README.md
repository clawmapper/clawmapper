# Roadmap Files

This folder contains the roadmap. It is written and maintained by the agent —
users interact with it through conversation, not by editing files directly.

---

## How it works

Tell the agent what you want recorded. It might be:
- A new initiative or project: "We're kicking off a payments overhaul in Q2, owned by Platform"
- A status update: "Self-serve onboarding shipped last Tuesday"
- Raw notes from a meeting: [paste] — the agent will extract and structure what's relevant
- A priority change: "Move the data export work to Q3, it's been deprioritised"
- Something cancelled: "We're dropping the desktop app, won't revisit this year"

The agent will write or update the appropriate roadmap file and commit it.

---

## File conventions

- **One file per period** works well: `q1-2026.md`, `h2-2026.md`
- **One file per squad or theme** also works: `platform.md`, `growth.md`
- The agent decides the file structure based on what makes sense for the content
- `_template.md` is the agent's internal reference for consistency — not for users to copy

---

## What this folder is not

- A task list or sprint board — keep that in your issue tracker
- A place for raw notes — paste those to the agent and it will structure them
- A place for stakeholder output — generated artifacts live in `outputs/`
