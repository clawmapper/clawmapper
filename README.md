# Clawmapper

This repository is a living product roadmap managed by an AI agent (Claude).

There is no application to deploy. The repo *is* the product — a structured set of
markdown files that the agent reads, writes, and maintains on behalf of the team.

---

## How to use it

**You don't edit files directly.** Instead, tell the agent what you want:

- *"We're kicking off a mobile redesign in Q2, owned by the Product squad"*
- *"Self-serve onboarding shipped last Tuesday"*
- *"Move the data export work to Q3 — it's been deprioritised"*
- *"Here are my notes from today's planning session: [paste]"*
- *"Make me a board slide covering Q1 progress"*

The agent will structure the information, update the roadmap, and commit the change.

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
