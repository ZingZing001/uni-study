---
course: SE761
type: project-artefact
title: Sprint 2 plan — first development sprint
date: 2026-08-16
source: Project_V4_6.pdf §3.2; SM sync with Jamuna 16 Aug; PO meeting 11 Aug
tags: [se761, project, sprint-planning]
---

# Sprint 2 — the first coding sprint

> [!important] Yes — Sprint 2 is where development starts
> Sprint 1 was the spike: planning, no production code. The project document (§3.2) says Sprint 2 must initiate development.
>
> **But Sprint 2 is not a free coding week.** It also carries the **Project Proposal**, the largest single document of the course, and the proposal depends on design decisions that must be made *this sprint*. Plan for roughly half the team's time going to design and documentation.

## What §3.2 requires by the end of this sprint

1. Architecture and domain model designed
2. Development environment set up
3. Database and initial data models set up
4. Mock-ups, wireframes and the initial theme (GUI projects — this is us)
5. Development activities initiated
6. Prototype developed if needed — **and thrown away before building the real system**
7. **Project Proposal submitted**

Plus: finalise and prioritise the product backlog, and finalise the high-level system blueprints.

---

## Sprint goal

> **A running, externally reachable skeleton that any team member can start a feature on, plus a Project Proposal that describes the system we actually intend to build.**

If both halves are true on Sunday, the sprint succeeded. Features can wait; the foundation cannot.

---

## Capacity reality check

Eight developers × roughly 6–8 development hours = **~50–60 hours**, minus the Scrum Master's 30% reduction.

The Project Proposal, use case diagram, architecture diagram, class diagram and wireframes will consume **20–25 of those hours**. Budget honestly: this leaves **30–35 hours of actual coding**. That is a foundation sprint, not a feature sprint.

> [!warning] The foundation trap
> Scaffolding is naturally two people's work while six wait. That is how a team ends Sprint 2 with six members holding zero commits on the default branch — and **individual contribution is assessed on exactly that**.
>
> Split the work deliberately into parallel tracks (below) so all eight land real commits this sprint. This is the single most important scheduling decision of Sprint 2.

---

## Carryover — close these first, they block everything

| Ticket | Why it blocks |
|---|---|
| **SCRUM-14** Tech stack | Blocks the dev environment, the database, the architecture diagram and the class diagram. **Decide at Tuesday's meeting, no later.** |
| **SCRUM-16** Definition of Done | Required in the Project Proposal, and every demo from Sprint 3 shows items "Done as defined in the Project Proposal" |
| **SCRUM-10** Release Plan Part 2 | Story points for the whole backlog. Do it at the Sunday planning session — velocity from Sprint 3 depends on it |
| **SCRUM-11 / 12 / 13** GitHub | Repo, UoA-verifiable accounts, all 8 joined with a first commit. **SCRUM-12 is the zero-mark one** |
| **SCRUM-7** Project Agreement | Week 3 deliverable, still open |
| **SCRUM-15** Board access | Story points + Reports enabled *before* planning; teaching team access before the proposal is submitted |
| **SCRUM-19** Evidence pack | Timesheet deadline announced; attendance sheet started |

---

## Proposed sprint backlog

### Track A — Foundation (target: done by mid-sprint)
| Ticket | Story |
|---|---|
| SCRUM-30 | Running front-end and back-end skeleton end to end |
| SCRUM-32 | Database schema managed by versioned migrations |
| SCRUM-98 | Whole stack runs locally with a single command (Docker) |
| SCRUM-31 | CI runs build, lint and tests on every PR |
| SCRUM-99 | Secrets and configuration kept out of the repository |

### Track B — Deploy early
| Ticket | Story |
|---|---|
| SCRUM-96 | System reachable from outside the university network |

Deploy the skeleton, not the finished product. **This project exists because the PO's current system is unreachable from outside the university network — proving we can do that in week one of coding retires the project's biggest risk.** Leave it to Sprint 6 and it becomes the thing that goes wrong at the final demo.

### Track C — Domain and data
| Ticket | Story |
|---|---|
| SCRUM-33 | Seeded demo data for patients, caregivers and prescriptions |
| SCRUM-44 | Create a patient record with basic details |

Seed data is worth more than it looks: every demo from Sprint 3 needs realistic content on screen in five minutes.

### Track D — Access control (start, finish in Sprint 3)
| Ticket | Story |
|---|---|
| SCRUM-35 | Caregiver or professional registers their own account |
| SCRUM-37 | Log in with email and password |
| SCRUM-38 | Role-based permissions enforced on every endpoint |

### Track E — Design and documentation (not Jira stories — proposal tasks)
- Use case diagram — high level, no syntax errors, PO-facing functionality only
- **Architecture diagram — logical application entities, NOT the tech stack.** "React Components / Front End APIs" is the exact wrong answer the FAQ calls out
- Conceptual class diagram with access modifiers and return types
- Wireframes and theme for the portal and the client — the theme should reflect the real final product
- Definition of Done, agile practices, meeting times, sprint start weekday, board link

### Stretch — only if the above lands
| Ticket | Story |
|---|---|
| SCRUM-81 | Visual ID behind an interface with a mock implementation |
| SCRUM-34 | README that builds and runs from a clean machine |

SCRUM-81 is cheap and unblocks the whole agent epic later. Worth pulling forward if there is room.

---

## Suggested split across eight people

| Pair | Focus |
|---|---|
| 1 | Backend skeleton + migrations (SCRUM-30, 32) |
| 2 | Docker, CI, secrets (SCRUM-98, 31, 99) |
| 3 | Frontend skeleton, theme, wireframes |
| 4 | Domain model, seed data, patient record (SCRUM-33, 44) |
| — | Deployment (SCRUM-96) — one person from pair 2, once the skeleton exists |
| — | Diagrams — split across pairs so each pair documents its own area |

Pairing keeps eight people productive on work that would otherwise fit two. **If pair programming is used, split the commits — take turns pushing, or only one of the pair gets credit.**

---

## Two meetings before the break

Only two team sessions remain before the study break, and Sprint 3's demo lands in Week 6.

| When | Purpose |
|---|---|
| **Tuesday 1–3 pm** | Close SCRUM-14 (stack). Ratify the DoD. Assign the tracks above. Everyone verifies their GitHub account is UoA-identifiable, on screen. |
| **Sunday 17:30** | Sprint 2 retro + Sprint 3 planning. Collect timesheets. Confirm the proposal is submitted. |

> [!warning] Sprint 3 closes before the study break
> The project document requires Sprint 3's backlog to be cleared and all its closure events held **before** the break starts. Sprint 3 also carries the first assessed Sprint Demo and the GitHub Repository Information Sheet plus ownership transfer. Do not let Sprint 2 work spill into it.

---

## Definition of sprint success

- [ ] Project Proposal submitted on time
- [ ] Tech stack confirmed and documented with a rationale
- [ ] Skeleton runs locally with one command, and is deployed somewhere reachable from outside the university
- [ ] CI green on every PR, branch protection enforcing review
- [ ] Database schema and seed data in place
- [ ] Wireframes and theme agreed
- [ ] **All 8 members have at least one commit merged to the default branch**
- [ ] Story points on the backlog, velocity recorded for the first time

---

## Risks

1. **Stack decision slipping past Tuesday.** It blocks the dev environment, the database, and two diagrams due in the proposal this sprint. If Tuesday ends without a decision, the SM should call it.
2. **The proposal eating the sprint.** It is 15 marks and it is due — but a proposal describing a system with no running code behind it reads exactly like what it is. Protect the coding tracks.
3. **Six people idle behind two.** See the foundation trap above.
4. **Fortnightly PO cadence.** The PO will miss every second sprint review. Send a written summary in the off weeks and keep his replies as acceptance evidence.
5. **Still unanswered by the PO** and now blocking real stories: patient data classification and ethics, confidentiality, hosting and who pays, reminder delivery mechanism, professional-account approval, CARE schema. **Hosting blocks SCRUM-96/97, which are in this sprint** — if there is no answer by Tuesday, deploy to a free tier under the team's control and revisit later.
