---
course: SE761
type: project-artefact
title: Release plan — Sprints 3 to 7
date: 2026-08-16
source: Project_V4_6.pdf §3, §5; PO meeting 11 Aug; product backlog SCRUM-21..100
tags: [se761, project, release-plan, sprint-planning]
---

# Release plan — Sprint 3 through the final demo

> [!important] You have four development sprints left, not five
> Sprints 3, 4, 5 and 6 are the coding sprints. **Sprint 7 is not a development sprint** — it is defect fixing, documentation, the final demo and the reflection report, and it collides with the Part IV final report. Anyone planning to finish features in Sprint 7 will fail twice.

## Calendar

| Week | Date | Sprint | Fixed deliverables |
|---|---|---|---|
| 5 | 17 Aug | **Sprint 2** | Project Proposal |
| 6 | 24 Aug | **Sprint 3** | Sprint 3 Demo · GitHub Repo Information Sheet · **ownership transfer to `rshahamiriuoa`** |
| — | — | **Study break** | No formal sprint. Optional shadow sprints |
| 7 | 14 Sep | **Sprint 4** | Sprint 4 Demo |
| 8 | 21 Sep | **Sprint 5** | Sprint 5 Demo |
| 9 | 28 Sep | **Systems Week** | **No SOFTENG 761 work at all** |
| 10 | 5 Oct | **Sprint 6** | Sprint 6 Demo · submit all sprint demo slides |
| 11 | 12 Oct | **Sprint 7** | Final Demo and Presentation · code submission · Reflection Report · SM Participation Report |

Two structural gaps to plan around: the **study break** between Sprints 3 and 4, and **Systems Week** between Sprints 5 and 6. Neither is a buffer you can spend twice.

---

## Capacity budget

Roughly **45–55 development hours per sprint** across eight people, after meetings and demo prep. Four sprints ≈ **190 hours** of feature work.

The backlog is 71 stories. Sprint 2 takes ~11. That leaves **~58 stories across four sprints — 14 or 15 a sprint.** They are small stories, but that is a full plate with no slack.

> [!warning] Plan to cut, and cut early
> The `could` stories will not all happen, and that is fine — the course explicitly expects teams to mark lower-priority stories out of scope rather than pretend. Cutting in Sprint 4 is a planning decision. Cutting in Sprint 6 is a failure.
>
> **First to go, in this order:** SCRUM-95 export · SCRUM-94 caregiver follow-up record · SCRUM-58 prescription conflict warning · SCRUM-50 patient photo · SCRUM-79 spoken reminders · SCRUM-95/92 adherence analytics depth.

---

# Sprint 3 — Week 6 (24 Aug) · first assessed demo

**Goal:** a logged-in user can manage patients and their caregivers. The first thing the class sees works.

| Track | Tickets |
|---|---|
| Finish access control | SCRUM-36, SCRUM-39, SCRUM-40, SCRUM-41, SCRUM-43 |
| Patient & caregiver management | SCRUM-45, SCRUM-46, SCRUM-47, SCRUM-49 |
| Care plan — start | SCRUM-51, SCRUM-52 |
| Carryover | anything unfinished from Sprint 2 |

**Drag into Sprint 3:**
```
SCRUM-36, SCRUM-39, SCRUM-40, SCRUM-41, SCRUM-43, SCRUM-45, SCRUM-46, SCRUM-47, SCRUM-49, SCRUM-51, SCRUM-52
```

**SCRUM-47 matters more than its size suggests** — one device per patient, enforced in the data model. It is the constraint that makes the double-dose scenario impossible, and it is a good 20 seconds of the demo.

**Demo content (5 min, 2 presenters):** first 2–3 minutes introduce the PO, the product and the use case diagram — this is the first time the class hears about your project. Then Sprint 3 plan, Done stories, velocity history, burndown, per-member participation.

**Also due this week:** GitHub Repository Information Sheet, and **ownership transfer to `rshahamiriuoa`**.

> [!warning] Sprint 3 must close before the study break
> The project document requires the Sprint 3 backlog cleared and all closure events held **before** the break. If review and planning are normally merged, split them this once: Sprint 3 closure with the PO in Week 6, Sprint 4 planning after the break.

---

# Study break — optional, and worth using deliberately

No formal requirement to work. The honest calculus:

- **On track?** Take time off. Weeks 10 and 11 are brutal and you will want the reserve.
- **Behind, or someone is still learning the stack?** This is the catch-up window, and the course says so explicitly.
- **Ahead?** Run two shadow sprints on Sprint 4 work and buy yourself slack for the Systems Week gap.

Decide as a team at the Sprint 3 retro rather than letting it happen by default. Whatever you choose, remember Part IV project work also lands here.

---

# Sprint 4 — Week 7 (14 Sep)

**Goal:** the care plan is complete and generates a daily schedule. The agent can fetch it.

| Track | Tickets |
|---|---|
| Care plan completion | SCRUM-53, SCRUM-54, SCRUM-55, SCRUM-56, SCRUM-57 |
| Portal core | SCRUM-59, SCRUM-60 |
| CARE mock | SCRUM-81, SCRUM-82 |
| Agent skeleton | SCRUM-68, SCRUM-69 |

**Drag into Sprint 4:**
```
SCRUM-53, SCRUM-54, SCRUM-55, SCRUM-56, SCRUM-57, SCRUM-59, SCRUM-60, SCRUM-81, SCRUM-82, SCRUM-68, SCRUM-69
```

> [!important] SCRUM-56 is the hinge of the whole system
> Schedule generation blocks the entire agent epic. If it slips, Sprint 5 has nothing to build on. Start it on day one and give it your strongest pair.

**Decision that must be closed by the start of this sprint:** how a reminder actually reaches the patient (PWA + Web Push / native Android / email or SMS). SCRUM-70 cannot be estimated until it is answered, and it is the core of the product.

---

# Sprint 5 — Week 8 (21 Sep)

**Goal:** the full patient loop works end to end — remind, identify, confirm, record.

| Track | Tickets |
|---|---|
| Agent core | SCRUM-70, SCRUM-71, SCRUM-72, SCRUM-73, SCRUM-76, SCRUM-77 |
| Identification | SCRUM-74, SCRUM-75 |
| Portal | SCRUM-61 |
| Care plan | SCRUM-48 |

**Drag into Sprint 5:**
```
SCRUM-70, SCRUM-71, SCRUM-72, SCRUM-73, SCRUM-74, SCRUM-75, SCRUM-76, SCRUM-77, SCRUM-61, SCRUM-48
```

**This is the heaviest sprint and the most demo-able.** A live reminder → face check → confirm → caregiver sees it, is the story the whole project tells. If anything gets cut, cut from the portal, not from this loop.

**SCRUM-75 (alternative identification) is not optional polish.** It is the accessibility fallback the PO asked for *and* the CARE-outage fallback — one mechanism, two reasons — and it is what stops a demo dying because an external service is down.

> [!warning] Systems Week follows immediately
> Week 9 is zero SOFTENG 761 work for BE(Hons) students. Sprint 5 must be genuinely closed on the Sunday, not "nearly done, we'll finish it next week". There is no next week.

---

# Sprint 6 — Week 10 (5 Oct) · last development sprint

**Goal:** the caregiver oversight loop closes, the product looks finished, and CARE integration is real.

| Track | Tickets |
|---|---|
| Adherence & oversight | SCRUM-89, SCRUM-90, SCRUM-91, SCRUM-92, SCRUM-93 |
| CARE — real integration | SCRUM-83, SCRUM-84, SCRUM-85, SCRUM-86, SCRUM-87, SCRUM-88 |
| Portal polish | SCRUM-63, SCRUM-64, SCRUM-65, SCRUM-66, SCRUM-67 |
| Deployment & docs | SCRUM-34, SCRUM-97, SCRUM-100 |

**Drag into Sprint 6:**
```
SCRUM-89, SCRUM-90, SCRUM-91, SCRUM-92, SCRUM-93, SCRUM-83, SCRUM-84, SCRUM-85, SCRUM-86, SCRUM-87, SCRUM-88, SCRUM-63, SCRUM-64, SCRUM-65, SCRUM-66, SCRUM-67, SCRUM-34, SCRUM-97, SCRUM-100
```

**That is 19 stories and it will not all fit.** Deliberate priority order if you have to choose:

1. **Portal polish (SCRUM-63–67).** Code Quality and Professionalism is 15 marks and names GUI quality, responsiveness, validation and navigation explicitly. It also feeds the holistic score across every deliverable.
2. **Adherence view (SCRUM-89, 90).** Without it the trust-based design has no visible safety net and the product story is incomplete.
3. **README and ops (SCRUM-34, 100).** "You may receive a zero for the project if we cannot execute your software."
4. **CARE real integration (SCRUM-83, 86, 87).** Only if CARE is actually available. The mock plus a published spec (SCRUM-88) is a defensible outcome and can be presented as one.
5. Everything else.

**Also due this week:** zip and submit all sprint demo slides.

---

# Sprint 7 — Week 11 (12 Oct) · wrap-up, not development

Be ready to present on **Monday of Week 11**.

- Defect fixing and polish only — no new features
- Final code submission on Canvas (must match the repo)
- Reflection Report (individual) — due Sunday
- Participation Report and Peer-Review — one per teammate, so seven each
- Scrum Master's Member Participation Report
- **Judge every other team's final demo and submit at least 5 peer-review forms, during lecture hours, from a UoA Google account.** Skipping this is a 30% penalty on the whole project mark

**Final presentation (20 min: 15–17 present, rest Q&A), all 8 presenting equally.** Required content: team and client intro · what the project is · product backlog with estimated *and actual* story points · final blueprints · complete software demo · what was not completed and why · agile process and practices adopted · velocity per sprint · proof of 560 team hours · proof of 70 hours per member · the SM Participation Report. Items 9, 10 and 11 must be consistent with each other.

---

# Presenter rotation — decide this now

Every member must present at least once across Sprints 3–6, or **they get zero for sprint demos**. Four demos, two presenters each, eight people.

**That is exactly enough with zero slack.** One illness breaks it.

| Demo | Presenters |
|---|---|
| Sprint 3 | ⬜ ⬜ |
| Sprint 4 | ⬜ ⬜ |
| Sprint 5 | ⬜ ⬜ |
| Sprint 6 | ⬜ ⬜ |

Fill the names in at the Sprint 2 retro and put it in the shared drive. Swap rule: if someone cannot present, they take the next slot and the swap is recorded — never silently dropped. Anyone who has not presented by Sprint 6 must be given that slot.

---

# Standing weekly rhythm

| When | What |
|---|---|
| Sunday 17:30 | Sprint retro + next sprint planning. Timesheets collected. Velocity and burndown updated |
| Monday | Sprint starts. SM sends the forecast table to the PO |
| Tue 1–3 pm | Working session / standup |
| Other days | One-line async standup in Discord |
| Wednesday | **Sprint demo in lecture time.** Book the slot in advance on the Sprint Demo Booking Sheet — no booking, late penalty |
| Fortnightly | PO meeting. Written summary to the PO in the off weeks |

---

# What must be true at each demo, from Sprint 3

Build the deck template once and reuse it:

1. Sprint plan of the sprint that just finished
2. Demo of stories marked Done per the Definition of Done in the Project Proposal
3. Velocity history — planned vs actual, bar chart
4. Sprint burndown chart
5. Explanation of any significant velocity change
6. Per-member attendance and participation

---

# Risks across the remaining sprints

1. **CARE never arrives.** Owned outside the team, still unfinished. Mitigation is already in the plan: mock first (SCRUM-81), fallback path (SCRUM-75/82), published spec (SCRUM-88). A working mock plus a spec is a defensible final-demo story. A hard dependency is not.
2. **Sprint 6 overloaded.** 19 candidate stories against ~50 hours. Use the priority order above and mark the rest out of scope in the final presentation — item 6 of that presentation asks for exactly that.
3. **The two gaps.** Study break and Systems Week both break momentum. Close each preceding sprint properly rather than carrying work across.
4. **Unanswered PO questions still blocking Must stories** — patient data classification and ethics, confidentiality, hosting and who pays, reminder delivery, professional-account approval, CARE schema. Reminder delivery blocks Sprint 5's core loop; get it answered by the Sprint 4 planning session at the latest.
5. **Uneven contribution surfacing late.** Check the GitHub Contributors chart at every retro, not in Week 11. Someone with no default-branch commits by Sprint 4 is a problem you can still fix; by Sprint 6 you cannot.
