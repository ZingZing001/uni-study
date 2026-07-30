---
course: SE761
lecture: 3
title: Agile and Scrum — one-page summary
date: 2026-07-27
tags: [se761, agile, scrum, summary, revision]
---

# 🌀 L3 — Agile and Scrum · one page

> [!abstract] The through-line
> Agile is a **characteristic** applied to a process. **Four values** generate **twelve principles**. **Scrum** is the process you get when you build from them. Client **needs** ([[../../Lecture2/notes/L2-notes|L2]]) become **user stories** → **acceptance criteria** → **tests** → the **product backlog** you burn down in sprints.

> [!bug] Source caveat
> No slide deck. Auto-transcript is **fair** — heavy student crosstalk garbling, and *Scrumban* → "scumbags", *Done* → "Donne", *product owner* → "Platonov". All diagrams in the full notes are generated, not the lecturer's.

---

## 1 · Agile is an approach, not a methodology `high`

Not a model/methodology/process — **a characteristic you apply to a process to make it agile or not**. "Agile" = quick, nimble. Reframe "do you use an Agile methodology?" as **"is your development process following agile thinking?"** Thinking is communicated as **values → principles → processes** (Scrum, Kanban, XP, Scrumban).

## 2 · The four values `high` — Assignment 2 ¶1

**X over Y** — both halves valuable; the value states the tie-breaker.

| Value | Left demands | Right side |
|---|---|---|
| Individuals & interactions | continuous communication; equal say; *no one leads, no one is left behind* | processes and tools |
| Working software | a build that compiles, runs, and is available to all | comprehensive documentation (the SRS) |
| Customer collaboration | PO engaged across all sprints (here: via sprint reviews) | contract negotiation |
| Responding to change | changes accepted mid-development, promised up front | following a plan |

## 3 · The twelve principles `high` — refer to **1–2 specific ones**, never "the principles"

- Highest priority: **early and continuous delivery of valuable software**
- **Welcome changing requirements, even late**
- **Deliver frequently** — manifesto says weeks–months; industry ~4 weeks; **this course = 1 week**
- **Working software is the primary measure of progress**
- **Face-to-face conversation** (principle 6) — *"may be online"*
- **Sustainable pace**

> ⚠ **The principles are not part of the contract.** They set the default posture; the PO conversation sets the actual limit.

## 4 · Working software + continuous integration `high`

**Working software = compiles + runs + available to the team.** Small changes → commit → build green → tests pass, so anyone can clone and work.

- Payoff 1: nobody is ever blocked.
- Payoff 2: **always demo-ready** — multiple working versions per day.
- Anti-pattern: days/weeks of local work then one big commit. Breaks the build **and** leaves no evidence you worked.
- **Commits are the best evidence of contribution.** A planning-only role leaves no trace and loses marks.
- XP practices named: **pair programming · code reviews · CI**. Code quality is separately marked — agree standards in meeting 1; 1–2 members may own review.

## 5 · Customer collaboration when the PO vanishes

**Be ahead of the game.** In meeting 1 establish (a) their availability for coming weeks, (b) *"if you're not available, can we go ahead, and how much?"* — anchored on a **draft product backlog**. Then *"we did talk about it"* → fewer grounds for complaint.

## 6 · Change vs scope creep

Two brakes: **(a)** say "changes wherever possible" up front — *"should not be that vast"*; **(b)** the PO **owns the end product**, so they want completion more than you do. Legit pushback: a late **technology** switch — *"be sceptical."* Change conversations belong in **sprint reviews**.

## 7 · User stories `high`

**As a `<who>`, I want `<what>`, so that `<why>`.** Requirements rewritten developer-friendly, one line. The *who* slot matters because different user types get different UI and different functionality. Requirement → many stories → prioritised into sprint backlogs. Tooling (Trello etc.) is your call.

## 8 · Acceptance criteria `high`

The **specific** version of a story — actual actor, actual content, actual stakeholders. Primary advantage: **easily translated into unit/integration tests**. Basis of **TDD** — write criteria before touching functionality.

> ⚠ **Code Runner trap:** ten visible tests → students pass all ten and stop, ignoring edge and boundary cases. **Criteria are a floor, not a ceiling.** How much testing is enough is a **PO decision**.

## 9 · Scrum `high` — Assignment 2 ¶2

**A lightweight framework defined around people and their communication.** Built from the values, especially individuals-and-interactions.

- **Scrum Master** — facilitator, *not* the leader; removes impediments. **"Everyone is a leader and there is no leader."**
- **Product Owner** — maximises the value produced by the dev team.
- **Developers** — self-organise by communication, not by dictation; **the team selects how much work it commits to.**
- Roles switch mid-sprint when someone is unavailable. Industry mixes Scrum, derivations, Kanban, Scrumban — inertia is the main factor: *"it is so difficult to change."*

## 10 · Three pillars `high`

| Pillar | Concretely |
|---|---|
| **Transparency** | Everyone's progress visible. Board per member + **Definition of Done** ticks. ⚠ **Opaque sub-groups** inside a big team break this — the default outcome unless tooling prevents it |
| **Inspection** | Review each other's work; regular code review |
| **Adaptation** | *"Very tricky"* — a member drops a technology, or the PO adds a requirement. **Is your team good enough to adapt?** |

## 11 · Maintenance types

| Type | Trigger |
|---|---|
| **Corrective** | Something is wrong (PO at review, or your own retrospective) |
| **Adaptive** | Environment/technology/team changed |
| **Perfective** | ⚠ **No trigger** — "the UI could be nicer" |

*"Only do what is required."* Perfective is acceptable **only if** the PO asked for creativity **and** the team knows you're doing it — i.e. it's a transparency failure, not a taste dispute.

## 12 · Events, artefacts, cycle `high`

| Event | Who | Inspects |
|---|---|---|
| Sprint planning | team | what/how for the coming sprint; prioritises the backlog |
| **Daily Scrum · 15 min** | dev team **only** — ⚠ **not the PO** | today's progress and blockers |
| **Sprint review** | team + **PO + stakeholders** | the **product** (increment); adapts the backlog |
| **Sprint retrospective** | team | **itself**; plans improvements |

**Artefacts:** product backlog (*ordered list of everything that might be needed*) · sprint backlog · **increment** (always working software) · **Definition of Done** (crafted by the whole dev team).

> **Increment**, not the velocity chart, is the artefact giving a transparent view of the **current state of the product**. Working software is continuous *during* the sprint; the increment is the artefact *at* the boundary.

**Burn-down rising** (work remaining increasing) → **address impediments and facilitate a team discussion on blockers.** Not: extend the sprint (wrecks later sprints) · reassign to "faster developers" (undefinable, demoralising) · cut scope mid-sprint.

## 13 · Teamwork risks

- **99% chance** someone falls ill. Someone may vanish entirely (his own tutor did, by midnight email).
- **Mitigation:** in an 8-person team, **work in pairs so everyone has one backup.**
- Uneven contribution is *"very common"* → commits are the evidence.
- Plan all of this in the **retrospective**, and **escalate early** — *"if you approach them in week ten, they won't be able to help."*

---

> [!tip] If you have five minutes before the assignment
> §2 (four values, exact wording) → §3 (name **two** principles specifically) → §9 (Scrum roles + "everyone is a leader") → §12 (review vs retrospective).
