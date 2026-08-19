---
course: SE761
type: meeting-minutes
title: Minutes — Standup, Sprint 1 close and Sprint 2 planning
date: 2026-08-18
attendees: full team (Sindhu joined twice — laptop + mobile; two members left early for classes)
scribe: Johnson
source: transcripts.json (314 segments, 03:04–04:24)
tags: [se761, project, minutes, standup, sprint-planning, sprint2]
---

# Minutes — Tuesday 18 August 2026

**Course Week 5 · closing Sprint 1 (spike) · planning Sprint 2**

Combined standup, Sprint 1 closure and Sprint 2 planning poker. Ran ~80 minutes.

> [!bug] Transcript quality
> Auto-transcript, low confidence on many segments. Names render inconsistently (Jamuna as "Jimuna"/"Jibuna"/"Chimuda", Hoseok as "hosel"/"Hoseok", Discord as "slap"). Several spoken dates are wrong — see the date correction below. Anything marked ⚠ needs verifying before it is acted on.

---

## 1. Working agreement — settled

| Item | Decision |
|---|---|
| **Standup** | **Tuesdays**, weekly. Progress check: what you did, what you're blocked on, walk through your solutioning. |
| **Sprint review + planning** | **Sundays 5:30pm**, virtual. Longer than standup. Planning poker for the next sprint. |
| **Sprint length** | One week. Sprint 2 starts this week, **ends Sunday 23 August**. |
| **Roles** | **None. Everyone is full-stack.** Rejected role allocation on the grounds that splitting eight people into fixed roles would be unbalanced. |
| Definition of Done | Document drafted by Jamuna, to be posted on Discord after the meeting. Everyone reads it and types "agree" in the channel; the ticket closes once all eight have. |

**Sprint-end day vs demo day.** Raised that the lecturer wants sprints ending Wednesday to line up with the demos. Resolved as: the Tuesday standup presents the previous week's completed work, which gives the team room before the Wednesday demo. Sprint boundary stays Sunday.

---

## 2. Solutioning tickets — the main process decision

Proposed by Johnson, adopted with an amendment.

**The practice:** before writing code for a user story, produce a *solutioning* artefact that records how you intend to solve it, scoped to the story's acceptance criteria.

**The method described:**
- Interrogate the ticket with an AI assistant first — explicitly instruct it to *ask you questions* about what it does not understand and to *not assume or invent* missing information.
- Ask for **two or three implementation options**, then evaluate them yourself and choose one. Do not accept the first answer.
- Present the chosen approach at standup. This is the peer-review point, and the moment conflicts between one person's ticket and another's surface.

**Rationale given:** ownership. A team project has to account for scalability, for how your feature interacts with everyone else's, and for leaving room for later work — none of which survives one-shot prompting. The solutioning record also becomes shared context: the next person (or their agent, via the Jira MCP) can read everyone else's solutioning before touching the codebase.

> [!quote] The load-bearing line
> "We should own whatever we have built."

**Amendment adopted:** a **comment on the user story** is acceptable in place of a separate solutioning subtask. Raised on the grounds that with many stories, subtasks will be forgotten. Both forms accepted.

**Existing pain point noted:** people leave tickets sitting in peer review and do not move them to Done. Johnson has been moving them manually.

---

## 3. Tech stack — backend decided by vote

| Layer | Decision |
|---|---|
| Frontend | **React + Vite** — treated as settled |
| Containerisation | **Docker** |
| **Backend** | **Java / Spring Boot**, by team poll |
| Database | ⚠ **Still not decided.** Mongo setup was mentioned in passing; the earlier working assumption tied the database to the backend choice. Needs an explicit decision. |

**Arguments recorded:** Spring Boot favoured for scalability, with Java's OO model cited as the reason. Node/Express favoured for performance and for being easier to configure and integrate. Johnson abstained from the vote to avoid producing a tie.

---

## 4. Jira and repository

- Board restructured; the backlog is planned out **to the end of October** by Johnson and Jamuna. Sprint 2 is deliberately the **skeleton/foundation** sprint.
- Optional extras parked in the backlog to pull in only if capacity allows — patient photo upload, blog.
- Columns: To Do / In Progress / In Review / Done, plus **Blocked** to be added. A future *Ready to Release* column with a release gate and squashed merge commits was discussed and deferred.
- ⚠ **Jira free tier caps at 10 members.** Eight members plus two GTAs fills it. Adding the PO or teaching staff needs a paid plan and therefore funding. Action: email the lecturer.
- ⚠ **Repository is not yet in an organisation and access is blocked on the lecturer.** Flagged in the meeting as the top priority — *"otherwise we cannot start working."*
- **Open: one repo or two.** Currently a single repo. Argument for splitting frontend and backend: fewer merge conflicts. Argument against: some tickets need both ends anyway. Leaning towards two, unresolved pending repo access.

---

## 5. Evidence pack — participation timesheet

Each member maintains their own timesheet: name, hours spent per user story, tasks completed.

- Template to be shared by Jamuna after the meeting.
- **Fill it in after every standup — by end of day Tuesday**, so no one shows up missing when it is inspected.
- Sprints 1–2: record meetings attended, hours, and the agenda completed. From week 3 onwards, add the tasks worked on.
- Meeting summaries are posted in the Discord *meeting summaries* channel and can be used as source material.

---

## 6. Sprint demos

- First assessed demo: **Wednesday 26 August** (Week 6). 5 minutes.
- Content: this sprint's plan, previous sprint's completed items, and what is still pending. Slides or a document; not necessarily a working build.
- **Booking order runs team 1 to team 11.** The team wants one of the first three slots — two members have classes 2–5pm on Wednesdays. Action: book early and try to jump the queue.
- **Roster:** Johnson to draft one. Everyone must present at least once across Sprints 3–6; only the final demo requires the whole team.
- Members are willing to swap or cover, subject to the person being covered agreeing.
- Noted: the demo is for assessment, not for the client. The PO may attend if they wish.

---

## 7. Product Owner

- PO has replied and is **satisfied with what was submitted**.
- ⚠ **Still no answer on the server questions.** Second sprint running. This now blocks a Sprint 2 ticket that requires deployment reachable from outside the university network.
- **MVP definition drafted** by Johnson — in Jira as **SCRUM-16**, with a more readable *MVP scope proposal* document in the Discord requirements channel. Deliberately written for the PO's comprehension rather than for developers.
- **PO meeting tomorrow (Wed 19 Aug).** If they already have structures in place, some tickets will need reworking — though the expectation is that little will change, since the backlog was built from the Hoseok conversation.
- **Ask for mock data tomorrow** — needed for the seeded demo data ticket.

---

## 8. Project Proposal

Due **Sunday 23 August**. Decision: draft it **after** tomorrow's PO meeting rather than before.

Raised and agreed: mock-up screens are worth producing regardless of whether the proposal strictly requires them, because they clarify what is being built.

---

## 9. Sprint 2 planning poker

**Estimation unit: story points read as hours**, agreed as more appropriate for one-week sprints. (Several 100-point votes appeared and were attributed to a bot or a stale page, not a real estimate.)

Sprint 2 is the skeleton. Stories estimated included:

| Ticket | Story |
|---|---|
| SCRUM-31 | Frontend and backend skeleton deployed, able to talk to each other |
| SCRUM-33/34 | Foundation items |
| SCRUM-35 | Caregiver or professional registers their own account — backend concerns: password hashing, duplicate email handling |
| SCRUM-37 | Login end-to-end, linking backend to frontend for a complete login service |
| SCRUM-38, 43, 45 | Estimated 3 each |
| SCRUM-44 | Healthcare professional creates a patient record with basic details |
| SCRUM-96 | Deployment — acceptance criteria require the project to be reachable **from outside the university network** |
| SCRUM-99 | Configuration item, settled at 2 |

Most estimates landed at 2–3. Seven or eight stories estimated in this session; the full backlog is 94 tickets and is **not** estimated in one sitting — it happens weekly.

**Design guidance given during estimation:** build for scalability and maintainability now. *"If we have a very painful design at the start, then it would be painful for us to try to change something six weeks in."*

**Task allocation method:** Johnson to sum the sprint's story points, divide by eight, and assign each member roughly equal points.

> [!warning] Unresolved
> A counter-proposal was raised late: split the team 2–3 frontend, 2–3 backend, 1–2 infrastructure per sprint, rotating every two weeks, to reduce merge conflicts. This partially contradicts the "everyone full-stack" decision in §1. The objection raised was that many tickets require both ends. **Not resolved — settle it at the Sunday planning session**, because it also determines whether the repo is split.

---

## 10. Date correction

> [!important]
> Several dates spoken in the meeting are wrong. "Sprint demo on October 11th" and "next week, 6th October" do not match the course schedule.
>
> **Correct:** Sprint 2 ends **Sunday 23 August**. Project Proposal due **Sunday 23 August**. First assessed sprint demo **Wednesday 26 August** (Week 6) — which is what was said later in the meeting and is right.

---

## 11. Actions

| # | Action | Owner | Due |
|---|---|---|---|
| 1 | Share the Definition of Done document on Discord; everyone reads and types "agree" | Jamuna → all | After meeting |
| 2 | **Chase the lecturer on repo/organisation access** — blocking all development | Jamuna | End of day |
| 3 | Share the participation timesheet template | Jamuna | After meeting |
| 4 | Everyone fills the timesheet weekly | All | End of day, every Tuesday |
| 5 | Email the lecturer re: Jira 10-seat cap and whether funding is available | Jamuna | This week |
| 6 | Approve the GTAs' pending Jira requests (admin action) | Jamuna | This week |
| 7 | Book an early sprint demo slot; draft the presenter roster | Johnson | This week |
| 8 | Post the meeting summary to Discord | Johnson | After meeting |
| 9 | Comment on SCRUM-20 with the outstanding PO questions; ticket rolls to next sprint | Jamuna | Before PO meeting |
| 10 | Ask the PO for **mock data** and chase the **server** answer | Team | PO meeting, 19 Aug |
| 11 | Close Sprint 1, configure the board for Sprint 2, assign tickets by equal story points | Johnson | After DoD signoff |
| 12 | Draft the Project Proposal | All | After PO meeting, due Sun 23 Aug |

---

## 12. Risks

1. **Repo access is the binding constraint.** Nothing ships until the lecturer grants it. It has been chased; escalate tomorrow if there is no reply.
2. **PO silence on servers is now two sprints old** and blocks the deployment story that is the core of the project's rationale. The project doc says to notify the course director if a PO is unreachable for more than two sprints — that threshold is close.
3. **Database undecided** while the backend is now fixed to Java. Decide before anyone scaffolds persistence.
4. **Full-stack vs specialised split is contradictory** as recorded. Two decisions in one meeting point opposite ways; resolve Sunday.
5. **Jira seat cap** may force either funding or leaving the PO off the board.
6. **Timesheet discipline** is the individual-mark protection for all eight. It only works if it is filled weekly from now, not reconstructed in week 11.
