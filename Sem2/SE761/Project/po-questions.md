---
course: SE761
type: project-admin
title: PO questions — Release Plan Part 1
date: 2026-08-05
source: Project_V4_6.pdf; Project/meetings/2026-08-04-minutes.md
tags: [se761, project, product-owner, release-planning]
---

# Questions for the Product Owner

> [!abstract] Status after PO Meeting 1 (11 Aug 2026)
> Sections A–D were used in the first PO meeting. **Answers are recorded in [[2026-08-11-po-minutes]]**, and the questions still outstanding are consolidated in section 7 of those minutes — data (real/synthetic/anonymised), confidentiality, hosting, CARE server readiness, role-view differences, missed-dose handling, PO availability, and a full capability ranking. Take those into PO Meeting 2 first.
>
> **Q4 below was answered in the negative:** the robot is *not* the only user. The web page for humans is the PO's first priority.

Domain (corrected 11 Aug): a healthcare platform where a phone or local machine acts as a **virtual agent** that reminds patients about medication and exercise, checks their visual ID, and reports interaction history to a server — alongside a **web page for healthcare professionals, caregivers and admins**, which is the PO's first priority. The agent does not administer medication; the model is trust-based.

> [!important]
> The PO was asked for **one hour per week**. Meeting 1 has to produce: project scope, **3–4 major capabilities**, and enough material to write the Product Backlog. Everything else is second-tier. Do not spend the hour on tech stack — they may not be a software engineer, and it isn't their decision.

**Suggested shape of the hour**
| Time | Segment |
|---|---|
| 5 min | Introductions, thank them for the project |
| 5 min | Our process, deliverables and schedule (one person, rehearsed) |
| 30 min | Section A + B below — vision, capabilities, priorities |
| 15 min | Section C + D — constraints, logistics |
| 5 min | Read back what we heard, confirm next meeting |

Nominate one scribe and one facilitator. Everyone else listens. Eight people talking at a PO is how an hour disappears.

---

## A. Scope and vision — ask these first

1. In your own words, what problem does this system solve, and for whom?
2. **If we deliver only one thing by mid-October, what must it be?** (This is the single highest-value question in the meeting.)
3. What does success look like to you at the end of the project — a demo, a deployed system, a research prototype, something you can show at a conference?
4. ~~Who actually uses this? We currently assume the **robot is the only user** and that any web UI exists purely so we can demonstrate the system. Is that right, or is there a human user — a nurse, a caregiver, a pharmacist, an administrator — who needs a real interface?~~
   **ANSWERED (11 Aug):** there are human users. Three roles — healthcare professional, caregiver, admin — and the web page serving them is the **first priority**.
5. What happens today, without this system? What's the manual process being replaced?
6. Is there anything you explicitly **don't** want us to build?

## B. Domain rules — this is where the user stories come from

7. Walk us through one complete medication round from start to finish, as it happens in reality.
8. What identifies a patient to the robot — facial recognition, a wristband, a room number, a scan? **Is that recognition something we build, or something that already exists and we call?**
9. What exactly is a "medication record"? Do we need to model prescriptions separately from administrations?
10. Who prescribes, and does the system need to capture that, or does it arrive from elsewhere?
11. How are doses scheduled — fixed times, windows, as-needed (PRN)?
12. **What must happen if a dose is missed, refused, or given late?**
13. **Safety scenario:** two robots approach the same patient at the same time. Robot A administers and saves; Robot B has already read stale state and is about to give a second dose. What should the system do — hard lock, reject, alert a human? *(This is a safety-critical requirement, not an implementation detail. Get the PO's answer in writing and turn it into a backlog item with acceptance criteria.)*
14. Does anything need human approval or override before a robot acts?
15. What has to be auditable — who administered what, when, and on whose authority?
16. Is there any alerting or escalation when something goes wrong?

## C. Constraints — ask before we design anything

17. **Real patient data, synthetic data, or anonymised?** If real, what ethics approval, privacy obligations, or data-handling rules apply to us?
18. **Is this project confidential?** It affects whether we can demo publicly in class and what we can put in a report.
19. Is there existing code, a previous year's project, a dataset, or a paper we should start from?
20. Is there real robot hardware, a simulator, or do we mock the robot entirely? **Do we get access, and when?**
21. If hardware exists — what does the robot speak? REST, MQTT, gRPC, a vendor SDK? Who writes the robot-side client, us or you?
22. Any technology we must use or must avoid — institutional standards, existing infrastructure, licensing?
23. **Hosting and servers: can you provide them, and can we start that request this week?** *(The course doc explicitly warns UoA servers take a long time to provision. Ask in meeting 1, not meeting 3.)*
24. Any budget for cloud, APIs or services, or do we stay on free tiers?
25. Who owns the IP, and what happens to this after the semester?
26. Scale we should design for — how many robots, how many patients, concurrent at peak?
27. Does the robot need to work offline or with unreliable network?

## D. Working relationship — logistics, keep it to five minutes

28. How much time can you realistically give us each week, and when?
29. Preferred channel for quick questions between meetings — email, Teams, Discord?
30. Would you like to attend sprint reviews in person, online, or receive a written summary?
31. Would you like access to our Jira board and GitHub repo? *(Both permitted.)*
32. Are there other stakeholders or domain experts we should talk to — a clinician, an end user, your research group?
33. Is there anyone who can answer clinical questions when you're unavailable?

---

## Ask these at the end, deliberately

34. **Prioritisation:** "Here are the capabilities we heard — can you rank them 1 to 4?" Make them do the ranking. Their priority order is the Product Backlog order, and the course explicitly makes backlog prioritisation the PO's job.
35. **Expectation setting** (say it out loud, don't imply it): seven one-week sprints, effectively 5–6 coding weeks, eight developers at roughly 6–8 development hours each per week. We'll commit to doing our best across as many features as possible, but we can't guarantee a complete solution. If we finish early, we'll come back and ask for more.
36. **Read back:** "So the three or four big capabilities are X, Y, Z — have we understood that correctly?" Confirming in the room is worth more than a follow-up email.

---

## After the meeting — same day

- [ ] Scribe writes up minutes and emails a summary to the PO: capabilities, priority order, decisions, and anything we said we'd do. Their silence on it becomes your written record.
- [ ] Turn answers into draft user stories with acceptance criteria (INVEST).
- [ ] Add Q13 (concurrency/double-dose) to the backlog as an explicit story, not a note.
- [ ] Log anything unanswered as an open question for meeting 2.
- [ ] Start the hosting/server request immediately if the PO confirmed one is needed.
