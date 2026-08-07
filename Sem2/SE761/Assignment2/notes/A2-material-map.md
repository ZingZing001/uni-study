---
course: SE761
type: assignment-working-note
assignment: 2
title: A2 — your own material, mapped to the rubric
tags: [se761, assignment, reflection, personal-material]
---

# 🗺 A2 — your material, mapped to the rubric

> [!warning] This note contains **no prose for the report.** A2 is a reflection; the brief says a ChatGPT-written one can be sent back to be redone, and the 3-mark block depends on things only you know. What's here is your own history sorted against the rubric, plus the questions you have to answer yourself.
>
> Sources: `runjiacv2026.json` (your CV export), your blog at `ZingZing001/PersonalWebsite-V2` (`src/data/blogPosts.js`), and [[A2-brief|the decoded brief]].

---

## ⭐ The structural insight worth building the report around

The brief names the constraint itself:

> *"…the context and constraints of a **university course** (which will have obvious differences to a real-world full-time industry job **where you are only focusing on one job at a time**)."*

**You are, right now, the extreme case of that.** Concurrently:

| Commitment | Role | Since |
|---|---|---|
| **EROAD** | Graduate Software Engineer, Tax team (part-time) | Nov 2025 |
| **AUSS** | Product Owner / Project Manager / Admin Secretary | Feb 2026 |
| **EVolocity capstone** | Team 22, 4 members | Mar 2026 |
| **UoA** | GTA, ENGGEN 299 | Dec 2024 |
| **SE761** | 8-person Scrum team, **one-week sprints** | now |

Most of the cohort will write about conflicting schedules abstractly. You can write about it as a **fact about your calendar**, and — more usefully — about what it does to *specific Scrum events*: daily scrums when you're at EROAD, sprint planning that has to survive four sets of availability, and a one-week sprint where being unreachable for two days is 40% of the sprint.

That connects straight to [[../../Lecture5/notes/L5-notes|L5]]'s risk #4 (conflicting schedules, mitigated by shared calendars and fixed weekly syncs) and #12 (dependency on key members).

---

## 🥇 The three strongest reflection candidates (3-mark block)

The rubric wants: **a previous experience → its actual outcome → how Agile would have changed it.** Ranked by how much only *you* could write them.

### 1. You have been the Product Owner ⭐ strongest

**AUSS.** You *"defined product vision, prioritised the backlog in Jira, and own end-to-end delivery"*, running *"sprint planning, code reviews, and stakeholder communication with the AUSS executive committee"* — with **student volunteer developers** and a **non-technical exec committee** as stakeholders.

In SE761 you flip to the other side: **a developer with an external, busy Product Owner.**

> [!important] Why this is the best material you have
> [[../../Lecture1/notes/L1-notes|L1-C04]] and [[../../Lecture3/notes/L3-notes|L3-C05]] are both about **what to do when the Product Owner is unavailable** — settle availability in meeting one, agree a proceed-without-you rule, never stop working. Everyone will recite that.
>
> **You have been the unavailable Product Owner.** You know why a PO goes quiet, what makes a developer's question easy versus expensive to answer, and what you'd have wanted your AUSS devs to do when you didn't reply.
>
> That's the definition of an insight the reader can't get from the Scrum Guide.

**Questions only you can answer:**
- When your AUSS devs were blocked on you, what did they actually do? What do you *wish* they'd done?
- Did you ever prioritise the backlog and get it wrong — and how did you find out?
- Your exec committee is a classic non-technical client. Did you hit **says vs wants vs needs** ([[../../Lecture2/notes/L2-notes|L2-C05]])? Which feature did they *ask* for that wasn't what they *needed*?
- Volunteers have no obligation to deliver. What did you use instead of authority — and does any of it transfer to an 8-person course team where nobody reports to anyone either?

### 2. EzShift — the project that didn't finish

**Feb 2025, third-year SWE students, "delivered using Agile methodology."** Your own CV then says: *"Next steps: **finalising the backend framework** and a scalable database schema."*

> [!warning] A year later, the backend framework isn't finalised.
> That is the most honest counterfactual in your history, and the rubric explicitly asks for *"previous development experiences **and their outcomes**."* An outcome that didn't land is worth more than one that did — provided you diagnose it rather than apologise for it.

**Questions only you can answer:**
- **What actually stalled it?** Motivation, schedules, a decision nobody made, or no forcing function?
- You had "modular implementation across HTML, CSS, JavaScript and JSON" but the backend was still pending. Was there ever a **working increment** — something demonstrable end to end? ([[../../Lecture3/notes/L3-notes|L3-C04]]: working software as the measure of progress.)
- Was there a **Definition of Done**? Would a one-week sprint with a demo at the end have forced the backend decision, or just produced a weekly excuse?
- It says "delivered using Agile methodology" — **was it?** Or was it iterative-ish with no events, no timebox and no PO? That gap between *calling it Agile* and *doing it* is [[../../Lecture3/notes/L3-notes|L3-C01]] (agile is an approach, not a methodology) with your name on it.

### 3. EROAD: the value that doesn't survive contact with tax

Your blog, on moving from the internship to the Tax team:

> *"The graduate role is a different kind of work… the bar isn't 'does the demo work?' but 'will this be correct, reliable, and maintainable for years?'… Moving from **'move fast and prototype' to 'move carefully and build to last'** has been one of the most valuable shifts in how I think as an engineer."*

> [!important] This is a genuine tension with an Agile value, not a caveat
> **"Working software over comprehensive documentation"** and *"deliver working software frequently"* sit awkwardly against compliance code where *"a subtle bug isn't just an inconvenience"* and behaviour *"has to be auditable."*
>
> And you're about to be pushed straight back to the prototype end: **one-week sprints, a spike in sprint 1, a demo in week 6.** You've lived both poles in the same year.

**Questions only you can answer:**
- Where exactly does "working software frequently" break down on the Tax team, and what does the team do instead?
- The **P1 billing incident** — unplanned work that arrives mid-sprint and takes priority. What did that do to whatever was already committed? (Scrum's sprint goal assumes the sprint isn't interrupted.) Your blog notes Travis and Mike *"doubled their workload to peer-review solutions"* — that's the sprint absorbing an interruption by burning slack that a student team doesn't have.
- Mike consulting Ramy under time pressure because *"we were there to correct data, not generate more problems"* — is that a Scrum practice, a values thing, or both? Does an 8-person student team have any equivalent?

---

## 🧩 Two more, if you need a fourth angle

**EVolocity capstone — the HTTP → MQTT migration.** Your CV: *"ESP32 firmware (ESP-IDF) **migrated from HTTP to MQTT**."* A protocol change mid-project, in a 4-person team, on a fixed academic deadline.

⭐ The interesting question is [[../../Lecture3/notes/L3-notes|L3-C06]]: **was that responding to change, or was it scope creep?** The distinction is that responding to change comes from the customer/problem; scope creep comes from the team. Which was it, who decided, and would a Product Owner have approved it? You also built *"a comprehensive Jest test suite covering unit, integration, SQL-injection and input-validation security tests"* — so you can speak to acceptance criteria becoming tests ([[../../Lecture3/notes/L3-notes|L3-C08]]) from experience rather than definition.

**Iking Tech, Nov–Dec 2024.** *"85+ hours of Agile methodology training, including daily stand-ups and mentor-led lessons… hands-on experience in **strict Agile workflows**."*

You have had **formal Agile training in a Chinese industry setting**, and you're about to do Agile in a NZ university setting. If anything from those 85 hours turned out to be context-dependent — a ceremony that worked there and won't work here — that's a strong, specific paragraph. Careful: only use it if you genuinely remember specifics, or it reads as CV padding.

---

## 🎛 The 1-mark criterion: Kanban / XP / other

The brief accepts **adopting or rejecting**, provided you justify it. You already practise several XP components:

| Practice | Where you already do it | Source |
|---|---|---|
| **Continuous integration / CI-CD** | Listed in your Cloud & DevOps skills; GitHub Actions on your portfolio | CV, blog |
| **Code review** | *"Run sprint planning, **code reviews**, and stakeholder communication"* | AUSS |
| **Testing discipline** | Jest suite incl. security tests | Capstone |
| **Kanban board** | **Jira** backlog prioritisation | AUSS |

> [!tip] The sharpest argument available to you
> [[../../Lecture5/notes/L5-notes|L5-C08]]: XP means taking a traditional good practice and doing it **continuously** — code review every sprint becomes **pair programming**, review all the time.
>
> You have an **8-person team** (large for Scrum) with **inconsistent skill levels** (L5 risk #5, mitigated by *"pair programming & knowledge-sharing sessions"*) and **one-week sprints**. That's a concrete case *for* pair programming — or a concrete case *against* it, if you argue eight part-time people can't afford to halve their parallelism. **Either argument scores; the unjustified one doesn't.**
>
> A Kanban angle that fits your situation: **WIP limits**, because your real constraint isn't ideas, it's the number of things eight partly-available people can have in flight at once.

---

## ⚙️ The 2-mark criterion: Agile values in a university context

Constraints you can name concretely rather than generically:

| Constraint | Why it bites *for you* |
|---|---|
| **One-week sprints** | Unreachable for two days = 40% of the sprint gone ([[../../Lecture5/notes/L5-notes|L5]] risk #2) |
| **Eight-person team** | Larger than Scrum's sweet spot; role clarity and decision-making get harder (risks #3, #6) |
| **Nobody full-time** | You have four other commitments; so does everyone else (risk #4) |
| **External, busy PO** | You've been on the other side of exactly this |
| **Sprint 1 is a Spike** | [[../../Lecture1/notes/L1-notes|L1-C06]] — the first sprint buys knowledge, not features |
| **No real Scrum Master authority** | Facilitation with no power over anyone's grade or time ([[../../Lecture1/notes/L1-notes|L1-C03]]) |

---

## ⚠️ Traps specific to you

> [!danger] 1. You have an unusually strong CV, and that is a hazard here
> This is a **reflection**, not a portfolio. Listing EROAD, AUSS, the capstone, Iking and the hackathon will burn 300 words and score in the wrong place. **Two experiences, deep, beats five experiences, listed.** The 3-mark line rewards *"reflective and insightful"*, not coverage.

> [!danger] 2. Don't let the good outcomes crowd out the instructive ones
> P1 resolved, agents shipped, pipeline built. Wins are harder to reflect on than failures, because there's no counterfactual — "and it worked" doesn't answer *"how might the outcome have changed if an Agile approach was followed?"* **EzShift is worth more marks than the P1 incident**, even though the P1 is the better story.

> [!danger] 3. Your writing voice is naturally promotional
> Your blog is warm and full of thanks-yous — which is right for a blog. The A2 rubric wants **reflective and insightful**, and the brief warns against reading as *"a series of pros and cons"*. Watch for sentences that describe rather than examine: *"This taught me the importance of teamwork"* is a description; *"I assumed X, then Y happened, so now I think Z"* is a reflection.

> [!danger] 4. You know more Agile than the assignment assumes — say the useful part
> You are a practising Product Owner with 85 hours of formal Agile training. Don't spend words proving you know the definitions; the rubric explicitly penalises *"merely repeating definitions."* The value of your background is that you can say **where the theory didn't hold**, which is exactly what the brief asks for.

---

## ✍️ A possible shape (yours to ignore)

Following Gibbs' Analysis spine from [[../../Lecture5/notes/L5-notes|L5-C02]] — *"how do past experiences compare to this?"* — one workable structure at ~850 words:

| ¶ | Content | ≈ words | Marks |
|---|---|---:|---|
| 1 | Open on the real constraint: five concurrent commitments, one-week sprints. Set up the question the report answers | 90 | writing |
| 2–3 | **EzShift**: what happened, why it stalled, and which specific Agile mechanism would or wouldn't have caught it | 260 | 3-mark block |
| 4 | **Being the AUSS Product Owner** — and what that predicts about being on the other side in SE761 | 180 | 3-mark + Scrum |
| 5 | Agile values against the university constraints; where you expect them to hold and where not | 180 | 2-mark values |
| 6 | **XP pair programming or Kanban WIP limits** — adopt or reject, with the 8-person/one-week reason | 100 | 1-mark |
| 7 | What you'll actually do differently, concretely | 60 | writing |

Note what's **not** in it: EROAD's AI agents, the hackathon, Iking, and the capstone. Cut them unless one earns its place by carrying an argument.

---

## ✅ Before you submit

Run the checklist in [[A2-brief|A2-brief.md]]. The two that matter most for your draft specifically:

- [ ] **Could a classmate have written this paragraph?** If yes, cut or specify it.
- [ ] **Is the past-experience block the longest section?** It carries 3 of 8 content marks.

> [!tip] Bring me the draft
> Once it exists I can check it against the rubric line by line, flag anything that reads as description rather than reflection, count the words, and tell you where it's thin — which is the part of this I can do properly.
