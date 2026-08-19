---
course: SE761
type: meeting-minutes
title: Minutes — Walkthrough of the existing robot app with Cole
date: 2026-08-19
attendees: Cole (existing robot team), SE761 team
scribe: Johnson
source: Screen-recording transcript (IMG_6265), 19 Aug 2026, ~9 min
tags: [se761, project, minutes, robot, reference-implementation, week5]
---

# Minutes — Robot app walkthrough with Cole, 19 August 2026

Cole is a developer on the PO's **existing** healthcare robot, not a supervisor and not the PO. He demonstrated the app currently running on the robot. Short session, ~9 minutes.

> [!important] Why this meeting matters more than its length suggests
> This is the first time we have seen a **working reference implementation** of the product domain. It gives us a concrete UI, a concrete feature set, and a concrete data model to align to — and it revealed a scope ambiguity we did not know existed. See §6.

---

## 1. The existing app — what is on the robot today

**Home screen sections:**

| Section | Contents |
|---|---|
| **Medication** | The taking flow: prompts the patient, "are you ready to take it now?", plus quizzes |
| **Reminders** | Reminder schedule and medication list with mark-as-taken |
| **Exercise** | Exercise videos |
| **Brain games** | Cognitive stimulation — explicitly designed for **elderly patients with dementia** |
| **Karakia** | Videos |
| **Entertainment** | Music, quotes, and dances (the robot moves its motors) |

**Test-only sections, not part of the product:**
- **Camera** — recently mounted hardware
- **Chat module** — LLM-based, still being implemented

### Reminders screen — the closest thing to a spec we have
- A time-ordered schedule: 8am have breakfast · 9–10am take medication · 3pm appointment
- The patient's medication list, each item markable as **taken**
- **Patient details panel** at the top showing basic information
- Reminders also fire as **notifications**; there is a test button to trigger them

> [!note]
> Marking medication as taken is self-report by the patient. This is the **trust-based model** the PO described, now confirmed in a working interface rather than in conversation.

---

## 2. Data and architecture, as it stands

- The robot app currently pulls from **a simple server the robot team built themselves**.
- They are **partway through integrating with the CARE server** and would ideally pull features from it — the chatbot module, and **face recognition, which they described as planned rather than built**.
- **The CARE server does not currently hold patient details.**
- Cole is still doing that integration himself and deferred the interface questions: **Finn and Jay** are the people to ask about the API contract — required headers, body format, JSON schema.

> [!bug] Risk confirmed, not reduced
> We recorded on 11 Aug that our mandatory visual ID check depends on the CARE server. Cole describes face recognition there as **planned**. A second, independent source now says the capability we depend on does not yet exist. Build against a mock and treat CARE integration as optional-path.

---

## 3. Domain rules learned

- **Doctors are the intended operators.** The intent is a doctor assigned to a patient, with the doctor assigning all medication the patient must take. The app is then the patient's medication reminder system.
- Right now none of this is enforced — the data is fake and nothing requires approval.
- **Unanswered:** whether there is a universal patient ID. Asked in the meeting, not addressed.

---

## 4. Missed doses — confirmed gap, and we were invited into it

We asked whether there is any flow for a patient missing a medication or an exercise — whether they are reminded again.

> [!quote] Cole
> "We don't currently have anything that does that, but that could definitely be something if you guys wanted to incorporate it."

Two things follow. The gap is **real and confirmed by the reference implementation**, and it has been **explicitly offered to us** rather than merely left open. This is the strongest available candidate for a feature that is genuinely ours, adds real value, and does not violate the PO's trust-based philosophy.

---

## 5. Mock data — contradictory answers, needs resolving

Within the same conversation:
- Asked whether they could provide full patient mock data → *"we can probably do that"*
- Later, asked where to get it → *"you might have to create your own mock data"*

Our position, stated in the meeting: we will generate our own data, but we want it **one-to-one with theirs** so the two systems line up. Cole agreed that would be preferable and suggested starting with dummy data regardless.

**Resolution needed:** get the existing server's schema from Cole or Finn, then generate our own data against it. Asking for their data is optional; asking for their **schema** is not.

---

## 6. The scope ambiguity — flag this before writing the Project Proposal

> [!warning] Two descriptions of the end state, and they are not the same project
> **Hoseok (11 Aug):** the existing university-hosted system is unreachable from outside, so we build a **new server** the group owns and can deploy freely.
>
> **Cole (19 Aug):** ideally there would end up being **one central server** that both the robot and our app pull data from.
>
> These may be the same thing — our new server *becomes* the central one — or they may be two different systems that need to reconcile. If it is the former, the existing robot app is eventually a client of what we build, which is a materially larger claim than "we build a web page and a phone client."

This belongs in the next PO conversation. The architecture diagram in the Project Proposal cannot be drawn honestly until it is settled.

---

## 7. Scope of the domain is wider than medication

The PO mentioned medication and exercise. The reference implementation also carries brain games, karakia, entertainment and appointments. **Karakia** is a te reo Māori prayer or incantation — a deliberate cultural-appropriateness feature for an Aotearoa eldercare context, not decoration.

We are not obliged to build all of it, but the Product Backlog and the use case diagram should show that we understand the product's full shape and have scoped deliberately within it.

---

## 8. Note on roles

Cole is a developer on the existing robot, not our client and not our supervisor. **Hoseok remains the PO.** The team observed in the meeting that the course's role mapping is awkward here — in a conventional setup the lab would be the client and the PO would sit between client and engineers — and that Hoseok's availability makes weekly contact difficult. Cole's advice was to keep checking in with Hoseok regardless.

Practical consequence: Cole is a useful **technical** contact for how the existing system works. He is not a source of requirements or priorities, and nothing he offers is a commitment.

---

## 9. Actions

| # | Action | Owner | Due |
|---|---|---|---|
| 1 | Contact **Finn and Jay** — CARE server API contract: endpoints, headers, body format, JSON schema, what exists today | TBC | This week |
| 2 | Request the **existing server's data schema** from Cole or Finn so our mock data matches one-to-one | TBC | This week |
| 3 | Resolve the **central-server ambiguity** with Hoseok before the architecture diagram is drawn | Jamuna | Before proposal |
| 4 | Ask Hoseok whether a **universal patient ID** exists or is expected | Team | Next PO contact |
| 5 | Add **missed-dose handling** to the Product Backlog as a candidate story with acceptance criteria | Johnson | Sprint planning |
| 6 | Reflect the full domain (medication, exercise, appointments, cognitive activities) in the use case diagram, with our scope marked explicitly | Team | Project Proposal |
| 7 | Keep the CARE dependency behind a mock; do not let any demo depend on face recognition being live | Team | Ongoing |
