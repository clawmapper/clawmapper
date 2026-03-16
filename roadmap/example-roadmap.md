# Roadmap — Q1 2026

_This is a worked example showing what a well-structured roadmap file looks like.
The agent creates and maintains files like this — you don't edit them directly._

---

## Overview

Q1 2026 is focused on improving new user activation and stabilising the platform
ahead of a planned marketing push in Q2. The Growth squad is running the activation
work; Platform is in reliability mode with a headcount freeze in place.

---

## Items

### Self-Serve Onboarding V2

- **Status:** in progress
- **Owner:** Product Squad
- **Quarter:** Q1 2026
- **Priority:** P1
- **Tags:** activation, onboarding, self-serve
- **Depends on:** Design system tokens (shipped Q4 2025)

**What:** Redesign the new user onboarding flow to remove the need for a human
setup call. Covers account creation through first meaningful action.

**Why:** Current trial → paid conversion is 12%. We believe 40% of drop-off happens
in the first 24 hours due to friction in setup. OKR KR1 targets 18% conversion.

**Success looks like:** Time-to-first-meaningful-action drops from 4 days to under 1.
Onboarding completion rate > 70% (currently 42%).

**Notes / open questions:**
- Waiting on UX research synthesis (due end of Jan)
- Mobile onboarding is out of scope for V2 — tracked separately

---

### API Rate Limiting & Observability

- **Status:** in progress
- **Owner:** Platform Squad
- **Quarter:** Q1 2026
- **Priority:** P1
- **Tags:** platform, reliability, api

**What:** Implement per-customer rate limiting on the public API and add
structured logging across all API endpoints.

**Why:** Two Sev-1 incidents in Q4 were caused by runaway API consumers. Without
rate limiting we can't safely grow API usage. OKR KR2: zero Sev-1 > 1 hour.

**Success looks like:** Rate limiting live for 100% of API customers. P99 latency
< 200ms sustained over 30 days.

**Notes / open questions:**
- Limit values TBC with Growth (don't want to throttle power users)

---

### Mobile Push Notifications

- **Status:** planned
- **Owner:** Growth Squad
- **Quarter:** Q1 2026
- **Priority:** P2
- **Tags:** mobile, retention, growth

**What:** Deliver transactional and digest push notifications on iOS and Android.
First use case: task completion reminders and weekly summary.

**Why:** Retention at 30 days is 38%. Comparable products see 15–20pt lift from
push. This is a quick win before the Q2 campaign.

**Success looks like:** 30-day retention lifts by at least 5 percentage points
among users who opt in to notifications.

---

### Data Export (CSV / PDF)

- **Status:** discovery
- **Owner:** Product Squad
- **Quarter:** Q1 2026 (stretch)
- **Priority:** P3
- **Tags:** product, compliance

**What:** Allow customers to export their data as CSV or PDF from the settings page.

**Why:** Recurring support request. Also a soft compliance requirement for some
EU customers. Low effort, moderate goodwill value.

**Success looks like:** Export available for all major data types. Support tickets
about data access drop by 50%.

**Notes / open questions:**
- Do we need to support custom date ranges, or is "all time" sufficient for V1?

---

## Shipped This Period

| Item | Owner | Shipped |
|------|-------|---------|
| Design system tokens V1 | Product Squad | 2025-12-18 |
| SSO (Google + Microsoft) | Platform Squad | 2025-12-05 |
| Bulk invite team members | Growth Squad | 2026-01-09 |

---

## On Hold / Cancelled

| Item | Reason | Owner |
|------|--------|-------|
| Native desktop app | Deprioritised — not in 2026 strategic bets | Product Squad |
| International payments | Blocked on legal review — Q3 revisit | Platform Squad |
