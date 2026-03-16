# Clawmapper

**AI-agent-managed product roadmaps. No app. No database. Just markdown, git, and Claude.**

You tell the agent what you're building. It structures everything, maintains consistency, and commits it to your repo. Stakeholders get generated outputs — slides, summaries, reports — on demand.

---

## Getting started

**1. Fork or clone this repo**

```bash
gh repo fork clawmapper/clawmapper --clone --remote=false
# or
git clone https://github.com/clawmapper/clawmapper.git my-roadmap
```

**2. Open it in Claude Code**

```bash
cd my-roadmap
claude .
```

**3. That's it — start talking**

The agent will introduce itself, set you up as admin, and ask what you'd like to work on. Tell it about your team, your projects, what's in flight. It handles the rest.

---

## How it works

**You don't edit files directly.** Instead, tell the agent what you want:

- *"We're kicking off a mobile redesign in Q2, owned by the Product squad"*
- *"Self-serve onboarding shipped last Tuesday"*
- *"Move the data export work to Q3 — it's been deprioritised"*
- *"Here are my notes from today's planning session: [paste]"*
- *"Make me a board slide covering Q1 progress"*

The agent structures the information, updates the roadmap, and commits the change.

---

## Repo structure

```
context/        Background docs — drop anything useful here (strategy, org info, etc.)
roadmap/        The roadmap files — written and maintained by the agent
outputs/        Generated artifacts (slides, summaries, reports)
templates/      Agent instructions for common output types
memory/         Agent memory and decisions log
roles.md        Who can do what
CLAUDE.md       Agent instructions (how this repo works)
```

---

## Roles

Access is managed in `roles.md`. The agent checks this before making any writes.
To add a team member, ask an admin to update that file.

| Role          | What they can do |
|---------------|-----------------|
| `admin`       | Everything, including agent instructions and roles |
| `squad_owner` | Roadmap and context files |
| `contributor` | Roadmap items they own |
| `viewer`      | Read access; can request outputs |
