# Roles

This file defines who can do what in this repository. The agent checks it before
making any writes. Admins should keep it up to date as the team changes.

For enforcement beyond the agent's honour system, configure GitHub branch protection
rules on `main` for `CLAUDE.md`, `roles.md`, and `memory/`.

---

## Users

| GitHub Username | Role          | Notes                        |
|-----------------|---------------|------------------------------|
| benfreeston      | admin         | Bootstrap admin               |

---

## Role Definitions

| Role          | Permissions |
|---------------|-------------|
| `admin`       | Full read/write access to all files including CLAUDE.md, roles.md, memory/ |
| `squad_owner` | Read all; write to roadmap/ and context/; cannot modify structural or memory files |
| `contributor` | Read all; write to roadmap items where they are listed as `owner:` |
| `viewer`      | Read only; can request outputs be generated but cannot commit anything |

---

## Adding a User

To add a team member, add a row to the table above with their GitHub username and role.
Only an `admin` may modify this file.
