---
course: SE761
lecture: 4
title: The paper-plane Scrum simulation — one-page summary
date: 2026-07-29
tags: [se761, scrum, sprint, velocity, estimation, retrospective, summary, revision]
---

# ✈️ L4 — Paper-plane Scrum simulation · one page

> [!abstract] The through-line
> [[../../Lecture3/notes/L3-notes|L3]] gave the definitions; this ran them. Four teams, two sprints, a Product Owner who changed the requirements mid-flight. **Every failure the class hit was one L3 had already warned about** — and that gap between knowing the rule and following it under time pressure is what **Assignment 2** asks you to reflect on.

> [!bug] Source caveat
> Workshop audio, so the worst transcript in the course. The lecturer's framed segments are intact; student contributions are patchy. **Sprint 2 numbers are incomplete** and marked as such — don't cite a figure for Team A.

---

## 1 · The mapping

| Game | Scrum |
|---|---|
| One accepted plane | one **story point** |
| Planes accepted per sprint | **velocity** |
| The lecturer | **Product Owner**, sole acceptance authority |
| 3 → 4 A4 sheets | fixed sprint resources |

**Timeboxes:** planning 3 min · execution 5 min · review flexible · retrospective 5 min. Teams of 3, each picking a **Scrum Master** to *"facilitate things and remove any obstacles."*

**Sprint 1 Definition of Done:** flies straight · no spin · up to 2 m · **pass/fail on aesthetics** (subjective, PO-owned — the one no test could anticipate).
**Sprint 2 adds:** hit a target · carry the company logo. **Additive — the old criteria still applied.**

## 2 · Estimation accuracy beats raw velocity `high`

| Team | Sprint 1 est → actual |
|---|---|
| A | 3 → **1** |
| B | 3 → **2** |
| C | 3 → **2** |
| D | **8 → 3** |

Team D built **nine** planes; three passed. Highest velocity overall, harshest verdict.

> *"The highest velocity is important. **But also the difference between what you estimated and what you ended up with**"* — and a repeated gap *"means there is some problem you need to discuss with your team during the review [and] retrospective."*

**Sprint 2 (partial):** D **5 → 6** (only clean figure, and the only team to beat its estimate) · B delivered 5 · C **0 accepted** (logo) · A ⚠ two conflicting statements, no number.

⚠ Last year's cohort made far more planes under near-identical rules — because **no-spin wasn't a criterion** and their planes were smaller. **Velocity isn't comparable across different definitions of done.**

## 3 · Sprint length is never altered

> **"An important aspect of Scrum is that we never alter the sprint lengths."**

Provoked by teams building during sprint 2's *planning* window; execution was cut to 3 min to compensate. Note the distinction: the **sprint boundary** is the fixed thing (it's what makes velocity comparable and lets a PO plan a release); the events inside are timeboxed for focus. Which is why sprint 1 and 2 here aren't strictly comparable — a demonstration of why the rule exists.

## 4 · Requirements changed mid-project, deliberately

Three changes: **+1 sheet** (*"because I need more products"*), **hit a target**, **company logo**. Labelled live: *"this is an example of change. A change in requirements."* Legitimate because it came with a **business reason**, was **additive**, and brought **more resources**. Prior planes were confiscated — no carry-over between sprints.

## 5 · Requirements are every member's job `high`

Team C: *"So what is your logo?"* → **"Oh, no logo."** → whole sprint rejected. **"All. All of you forgot."**

> *"Every individual of the scrum team has the responsibility of understanding all the requirements — **it should not be a responsibility of just the Scrum Master.**"*

Three people could have caught it; none did. That's **structural**, not carelessness — if everyone assumes someone else is tracking requirements, nobody is. It's the **inspection** pillar failing. Project corollary: *"even if 1 or 2 team members do not understand how Scrum works… that is going to create a big problem later."* No **fake or dummy members**.

## 6 · Test in something that resembles production `high`

Teams were told they could test anywhere. Sprint 2 put a target on the wall. **Nobody practised against it.**

> *"No one tried to actually simulate the actual environment, **which was right in front of you**."*

Student's own framing: *"[like we] ran the product into prod environment and it didn't work as expected."* Everyone tested that the plane *flew*; nobody tested that they could *hit the thing* — different rigs, and the second was inferred from the first. Compare the **Code Runner** trap (L3-C08): there you test only what's asked, here only what's convenient. Both give a green suite and a failed demo.

> *"If something fails on the first try, **the client is going to be bothered about it**"* — a failure in front of the customer costs more than the identical failure found privately.

## 7 · Self-organising: switch roles between sprints

**Team B, sprint 1:** SM + 2 devs + dedicated QA → *"due to the time crunch we were not able to complete the three products."*
**Sprint 2:** *"we **all became the developer** — being an agile team."* → recovered the aesthetics criterion they'd failed.

> Triggers: *"if something is not working with one of the team members… [or] if one of the team members is not available, then you can switch the roles."*

The point: a dedicated QA is the **wrong shape for a 5-minute sprint** — the specialist was idle while construction was the bottleneck. Self-organisation responds to *observed* bottlenecks, so you need a retrospective to observe them in.

## 8 · Converge on one design

Standardised: B, D. Experimented: A, C.

> **"Commit to one design, or at most two"** — expertise in one beats being *"a jack of all designs."*

Mechanism is a **process** failure: *"every developer was given this freedom to come up with their own design"* — a design is agreed to be good and the alternative is carried anyway. **Explore in sprint 1, converge by sprint 2** (Team A did exactly this and improved). On a real project: technology and architecture choice.

## 9 · Onboarding costs sprint time

Two teams gained a member after starting. *"You would have spent at least some time to talk to them and introduce them."* This is normal — *"that will also happen during your actual sprints."* Two obligations: **catch them up**, and **get them productive**, not merely informed. Cost is charged to the sprint's timebox, i.e. to the estimate. Cheaper if everyone has a designated backup (L3-C13).

## 10 · Retrospective before planning `high`

Corrected live: *"it would be better if we **first do sprint retrospective and then… sprint planning**. Which is more natural."*

```
Sprint → Review (product) → Retrospective (team) → Planning → Sprint
```

The retrospective's output **is** the next planning session's input. Reverse them and the findings sit unused for a whole sprint. Sprint 2's retrospective was replaced by the collective class debrief.

## 11 · Everyone is a leader and there is no leader `high`

> *"There is no leader. Scrum Master is just a **facilitator**."*

The honest cost: *"if there are a lot of views coming in from everyone, then **you need a consensus**."* With nobody entitled to decide, decisions require real agreement — which requires everyone to have understood everyone else. §8's four-designs problem **is** a consensus failure: nobody could say "we're using this one."

SM's job, as a verb list: **keep looking, reviewing, tracking, monitoring.** Not *decide*, *assign* or *approve*.

## 12 · The PO is part of the system too

Two admitted mistakes: **no restriction on building during planning** (forced the timebox cut), and **no test material supplied** (last year there were spare sheets for testing) — *"that's a product owner's problem. **I accept my mistake there.**"* Teams burned production material on experiments, which plausibly drove the sprint 1 estimate gaps.

**A retrospective's target is the whole system** — team, requirements, resources, and how the customer runs the engagement — not just the team's own behaviour.

*"**Pilot error**"* = a defect in the demo, not the product. The customer can't tell the difference and shouldn't have to.

---

> [!tip] If you have five minutes before Assignment 2
> §2 (the estimate gap) → §5 (Team C's logo) → §6 (nobody tested the target) → §10 (retrospective before planning). Those four give you **concrete experience to reflect on** rather than theory to restate — which is exactly what the rubric rewards. Assignment 2 brief in full: `../context/admin-and-dates.md`.
