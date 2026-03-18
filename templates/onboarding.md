# Clawmapper Onboarding Script

_This script is invoked by the agent on first session, after the admin bootstrap.
Run it as a conversation — wait for the user's answers before proceeding.
Record everything learned in `memory/MEMORY.md` before the session ends._

---

> **Welcome to Clawmapper.**
>
> I manage your roadmap — you talk, I write. Every change is a commit. Nothing lives outside this repo.
>
> Before we start, a few quick questions. Answer however you like — bullet points, sentences, a brain dump. I'll handle the structure.
>
> **1. What's the team or product I'm helping you manage?**
> *(e.g. "We're a 12-person product team building a B2B SaaS platform")*
>
> **2. Who are the key stakeholders I should know about — and what do they care about?**
> *(e.g. "Board wants revenue impact, engineering wants scope clarity, our CPO reviews monthly")*
>
> **3. Anything already in flight? Give me a rough sense of what's being worked on right now.**
> *(Don't worry about format — I'll ask follow-up questions to fill in the gaps)*
>
> Once I have this I'll set up your first roadmap file and we'll go from there. You can also skip any of this and just start telling me what to record — we can always fill context in later.

---

> **One thing worth knowing:** I'm instructed to commit directly to main — no branches,
> no PRs. Occasionally I may create a branch out of caution. If that happens, just tell
> me: *"Commit directly to main"* and I'll do that going forward.

---

## What to record in memory after onboarding

Once the user has answered, write the following to `memory/MEMORY.md` before the end of
the session. Use clear headed sections and date-stamp the entry.

- **Team / product** — what they're building, size, context
- **Stakeholders** — who they are, what each one cares about, how often they need updates
- **Current work** — what's in flight, even if rough (you'll formalise this in a roadmap file)
- **Output preferences** — any format or tone preferences mentioned (e.g. "board likes one-pagers")
- **Standing instructions** — anything they said that should shape how you work with them ongoing

If the user skipped questions, note what's unknown — a future session should prompt to fill the gaps.
