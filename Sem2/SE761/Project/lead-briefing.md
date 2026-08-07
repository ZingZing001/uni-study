---
course: SE761
type: project-admin
title: Points to guide the team on (senior member briefing)
date: 2026-07-29
source: Project_V4_6.pdf; Lecture1 admin-and-dates.md
tags: [se761, project, leadership]
---

# What to make the team understand early

Ranked by how much damage getting it wrong does.

## 1. The mark is one mark, not seven
Assessment is explicitly **holistic**. "If you have the perfect project proposal but you deliver a very crappy project, you will end up with a low holistic score." Code quality alone (15 marks nominal) drags the *entire* project score. Marks are released in one batch at the end. So there is no such thing as "the proposal is done, that's 15 in the bag."

**Implication to sell:** we optimise for a working, feature-rich, well-engineered product, and the documents describe it honestly. We do not optimise document-by-document.

## 2. Nobody hides. Three independent evidence streams
- GitHub contribution **to the default branch** (work stuck on unmerged branches counts as no contribution — FAQ 28)
- Scrum Master's weekly participation report
- 7 confidential peer reviews per person

**"Lack of code participation in the project will result in a zero mark for the entire project."** Non-coding roles do not exist here. People have failed this course while their teammates got A+.

## 3. GitHub hygiene is a zero-mark trap, not a style preference
- Account must be UPI-verifiable (public UoA email). Failure = **zero**. This already cost two students last semester.
- Repo private, correct name, all members + GTAs added, ownership transferred to `rshahamiriuoa`.
- **Continuous, meaningful commits from week one.** Bulk end-loading, fake commits, or add-then-delete padding = at least **30% deduction**, possibly zero.
- Pair programming? **Split the commits** — take turns committing, or only one of the pair gets credit.
- Canvas is the submission system. The repo is not a submission.

## 4. Scope is our job, not the PO's
Many POs are not software engineers and get ~1 h/week. **We** write the product backlog and user stories from what they tell us. **We** are responsible for making the scope big enough for a 700-level course and small enough to actually finish and test. Getting this wrong lowers the holistic score across every deliverable. Push back on the PO in both directions — that negotiation is literally being assessed.

Frame to the PO in meeting 1: seven sprints, effectively 5–6 coding weeks, we commit to doing our best across as many features as possible, no guarantee of a complete solution — and if we finish early we'll ask for more.

## 5. Design decisions that are being marked, so decide them deliberately
- **Object-oriented by default.** OO principles are explicitly evaluated in the holistic assessment; non-OO systems have to substitute activity/component diagrams and lose the class-diagram credit.
- Architecture diagram must show **logical application entities**, not the tech stack. "React Components / Front End APIs" is the exact wrong answer given in FAQ 25.
- SOLID + design patterns, named and visible.
- Automated tests, exception handling, input validation — assessed under Code Quality.
- If there's a GUI: consistent professional aesthetic, responsive, real validation, sensible animations. Mock-ups in the proposal should reflect the actual final theme.
- A README that lets a marker build and run it. **"You may receive a zero for the project if we cannot execute your software."**

## 6. Process artefacts are assessed, not optional ceremony
Compulsory: weekly sprints, sprint planning, frequent standups, user stories **with acceptance criteria**, product + sprint backlogs, sprint review, retrospective. Optional: pair programming, WIP limits.

The velocity chart, burndown, forecast tables and attendance sheets are demo content every single week. Build the deck template and the spreadsheets once in Sprint 1; after that it's five minutes a week. Teams that improvise this weekly lose demo marks steadily.

## 7. Calendar traps
- **Study break:** Sprint 3 must be *fully closed* before it starts. Officially no work required — but this is where a behind team catches up, and where members learning a new stack should catch up.
- **Systems Week (week 9):** zero SE761 work. Plan around a dead week.
- **Sprint 7 is not a development sprint.** It's polish, defect fixing, docs, final demo, reflection — and it collides with the Part IV final report. Anyone planning to "finish the features in sprint 7" will fail both.
- **Final demo attendance and peer judging:** at least 5 peer-review forms submitted **during lecture hours** from a UoA Google account. Skipping = **30% penalty on the whole project mark.** This is the cheapest 30% anyone will ever lose.

## 8. GenAI — the line, stated plainly
Permitted and expected as assistance; **must be disclosed** where it significantly contributed. But:
- You are 100% responsible for every line, including code a teammate or an AI wrote.
- Mandatory technical interviews may be called during the exam period to establish code ownership. Not attending = zero and/or misconduct.
- "The AI suggested this" is explicitly not an acceptable answer in Q&A.
- Wholesale AI-authored code or report = **zero**, possible disciplinary action.

**Team rule to propose:** no one merges code they cannot explain line-by-line at a whiteboard. Enforce it in code review.

## 9. Escalate early or not at all
"If you contact us week ten there is nothing that we can do." PO gone dark for more than 2 sprints → tell the course director and keep building to the release plan. Never stop the project.

---

## How I'd position myself (you)
- **Don't automatically take Scrum Master.** It's a 30% dev reduction, and it's mostly admin: charts, attendance, forms, submissions. If you're the strongest engineer, your marginal value is higher in architecture, code review and unblocking people. Take it only if nobody else can be trusted with the paperwork — because the paperwork failing hurts everyone's mark.
- **Do claim the technical spine:** architecture and domain model, repo/CI conventions, Definition of Done, code review standards, and the "can you explain this?" bar.
- **Deliberately don't hoard the interesting work.** Every member needs default-branch commits and needs to be able to explain the code. Pair the weaker members onto real features early rather than letting them drift into "documentation" — that's the failure mode that produces the individual zeros.
- **Set the Definition of Done with teeth in Sprint 1** (merged to default branch, tested, reviewed, acceptance criteria met, deployed/runnable). Every demo hangs off it.
