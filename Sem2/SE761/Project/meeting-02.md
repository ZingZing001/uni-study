---
course: SE761
type: project-admin
title: Team Meeting 2 — Week 3, post-allocation
date: 2026-08-05
source: Project_V4_6.pdf
tags: [se761, project, scrum, meeting]
---

# Team Meeting 2 — Week 3 (project allocated)

**Done:** EoI, Team Portfolio, Scrum Master (Jamuna), weekly meeting slot, project allocated.
**Outstanding:** GitHub repo, Jira/Trello board.

> [!important]
> The two outstanding items are **Sprint 1 gating requirements** — every member must have *joined* the repo by the end of Sprint 1 (week 4) or late penalties apply. They're an hour of work. The real critical-path item is **getting the PO into a room**, because that lead time isn't ours to control.

---

## Critical path — before the meeting ends

1. **Email the PO today.** Release Plan Part 1 must happen in week 3 or early week 4. Propose two or three concrete slots; don't ask an open "when suits you". Attach the Team Portfolio.
2. **Project Agreement** signed by all 8 and submitted on Canvas — week 3 deliverable.
3. Repo and board created **today**, not "this week".

---

## Agenda (60–75 min)

| Time   | Item                                                                 | Output                                         |
| ------ | -------------------------------------------------------------------- | ---------------------------------------------- |
| 5 min  | Confirm Project Agreement signed by all 8                            | Canvas submission                              |
| 10 min | Draft and send the PO email — write it together, send before leaving | Meeting booked / awaiting reply                |
| 10 min | **GitHub setup** — Jamuna creates it live on screen                  | Repo exists, invites out                       |
| 10 min | **Board setup** — Jira vs Trello, decide in 2 min, then build it     | Board exists, PO + GTAs invited                |
| 15 min | **Read the project brief together**, out loud                        | Shared understanding, question list for the PO |
| 10 min | Tech stack straw poll + skills audit                                 | Candidate stack, gaps named                    |
| 10 min | Working agreement                                                    | Standup cadence, DoD draft, review rules       |
| 5 min  | Assign owners and dates for everything above                         | Board populated                                |

---

## GitHub — do it live, get it right first time

- Private repo, named exactly `202X SOFTENG761 Project Team X` — **must match the Canvas name**
- Add all 8 members + both GTAs (`h-yamani`, `Rabia24-sudo`). PO optional but allowed
- **Every member, on screen, right now:** GitHub Settings → Emails → turn OFF "keep my email addresses private" → Public profile → set public email to their UoA address. Non-verifiable account = **zero for the project**
- Transfer ownership to `rshahamiriuoa` (week 6 deliverable — but do it once the repo is stable)
- Complete the GitHub Repository Information Sheet on Canvas when due (week 6)
- Default branch protection: PR + at least one review before merge. This is what makes "everyone contributes to the default branch" actually happen

## Board

Jira or Trello — either satisfies the requirement. Jira gives burndown and velocity charts for free, which are mandatory demo content every week from Sprint 3; Trello means building those by hand. Decide fast, don't debate it for 20 minutes.

Must be live and current at all times, with PO and teaching team access. The board link goes in the Project Proposal.

---

## Preparation for the PO meeting (Release Plan Part 1)

Assign an owner to each before the meeting happens:

- [ ] Read the project brief; write down every ambiguity as a question
- [ ] One person prepares a 3-minute "here's our process, deliverables and schedule" explainer for the PO
- [ ] Ask the PO about: servers/hosting (start early — UoA servers are slow), data access, existing code, who the end users are, what "success" looks like
- [ ] Expectation-setting line to deliver: seven one-week sprints, effectively 5–6 coding weeks, we'll do our best across as many features as possible with no guarantee of a complete solution — and if we finish early we'll ask for more
- [ ] Come out with **3–4 major capabilities** and a first-pass product backlog of user stories

---

## Working agreement to settle now

- **Standups:** frequency, time, format (async in chat is acceptable; must be documented)
- **Definition of Done** draft: merged to default branch, reviewed by one other member, acceptance criteria met, tests written and passing, runnable
- **Hours logging:** every member logs hours per sprint and reports to Jamuna weekly — set a recurring Friday reminder. 70 h per person by the end
- **Attendance sheet:** Jamuna starts it today, for every meeting and standup
- **Pair programming rule:** if used, split the commits — take turns, or only one of the pair gets credit
- **Explain-it rule:** nobody merges code they can't explain line-by-line. This is the defence against the mandatory technical interviews and the GenAI policy
