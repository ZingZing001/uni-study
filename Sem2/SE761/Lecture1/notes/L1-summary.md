---
course: SE761
lecture: 1
type: summary
title: L1 one-page summary — course intro, Scrum roles, imposter/DK
tags: [se761, revision, cram]
---

# ⚡ SOFTENG 761 L1 — one-page summary

> [!warning] ~75% of this deck is administration. Only the conceptual residue is here; logistics live in `context/admin-and-dates.md`.

## 🎓 What the course assesses

**Two axes: (1) how well you followed the process, (2) product quality + feature richness/complexity.**
> "It's not that your product works… That's not the only requirement."

Agile & Lean focus: **process and practices, self-organizing teamwork, project management** → high-quality software. Full lifecycle capstone: requirements elicitation → deployment. *"The best way to learn how to do agile is to do it."* Standard applied: **"We look at you as professional software developers."** No final exam.

## 📊 Bloom ladder — Course Design (Revised, 2001)

Remembering Fundamentals → Understanding Examples → **Applying in Simulations and Project → Analyzing Experience → Evaluating Practice → Creating an Agile Mindset**

Bottom two = "Less"; **top four = "More"**. The apex is a **mindset**, not knowledge.

## 🏃 Scrum Master ≠ project manager

> "Agile teams are **self-managed. There is no team lead** or anything."

Is: someone who **champions Agile principles and ensures they are actioned and realised**. Maintains the weekly member participation report. Expected to **code less**. Pick someone with Agile, else industry, experience.

## 👤 Product Owner vs client

| | Prescribed Agile | This course |
|---|---|---|
| PO is | a software developer | **PO + client fused** |
| Technical? | yes | often **not at all** |
| You must | take direction | also **translate terminology and expectations** |

PO **brings requirements and decides weekly which features to implement**. You help them **find what they need** and **prioritise**.
**If the PO becomes inaccessible: continue. The one thing you cannot do is stop.** A new version ships every week regardless.

## 🔄 Sprint structure

**7 sprints · each one week · fixed, non-negotiable.**

**Cycle:** a. Sprint Planning → b. Sprint Development → c. Sprint Review → d. Sprint Retrospective → e. Sprint Demo → *(repeat)*

| Sprint | Week | Content |
|---|---|---|
| **1 — Spike** | 4 | Release Planning Pt 1 & 2; **Product Backlog**. Only sprint not requiring new software. |
| 2 | 5 | System modelling & design; Project Proposal |
| 3–6 | 6–10 | Full cycle, each ending in a Sprint Demo |
| 7 | 11 | Final Demo & Presentation; Reflection Reports |

**Sprint 7 is not a development sprint** — polishing only; Part IV reports are due the same week.
**Spike** = investigate, decide back end / technologies / database, build the backlog.

## 😰📉 Imposter syndrome ↔ Dunning–Kruger

**Imposter syndrome** = *"the feeling that you're a fake and somehow you snuck in and you don't deserve to be where you are."*
Prevalence claim: **"if you don't experience imposter syndrome, that's abnormal."** Reframe: it signals **volume of new information**, not inadequacy.
**Strategy — do the simplest thing.** A project is a **puzzle**: *"every piece you put in place opens up opportunities to solve the rest."* Progress generates the information you lacked.

**Dunning–Kruger.** Origin: **MacArthur Wheeler**, 19 Apr 1995, robbed a bank wearing **lemon juice** believing it made him invisible to cameras — *"But I wore the juice."* **Dunning & Kruger** studied him. Finding: **people with low ability paradoxically overestimate themselves.**

| Stage | Monologue | Landmark |
|---|---|---|
| Start | "I know everything about this" | 🏔 **Mount Stupid** |
| Learning | "It's more complicated than I thought" | ↓ |
| Deep | "I'll never understand this!" | 🕳 **Valley of Despair** |
| Recovering | "It's starting to make sense" | ↗ |
| Competent | "Trust me, it's complicated!" | earned |

Two traps: **stop early → stranded on Mount Stupid**; **quit in the Valley thinking you learned nothing**.
Debate illustration: simpleton (loud, confident) beats student (knows more, silent, no confidence) and teacher (confident but hedges) — **"people tend to trust certainty."**
Culture: 93% of Americans vs 69% of Swedes think they're above-average drivers; Japan tends to underestimate. Socrates: *"I know that I am intelligent because I know that I know nothing."*

> [!important] **The integrative point**
> **"If you start the project and you don't feel imposter syndrome, you should be worried"** — it means you haven't understood the project or lack the knowledge to see what's ahead. **"If you don't expect it, maybe you are getting stuck on Mount Stupid."**
> Imposter syndrome = normal and good. Dunning–Kruger = "completely wrong."

## 🤖 Gen AI — Two-Lane Approach, **Lane 2 (uncontrolled)**

**Three pillars (Module 3):**
1. **Disclose** — significant GenAI contribution to a code block or report section must be declared; failure = academic dishonesty, investigated as plagiarism.
2. **100% responsibility, per student, for every line and paragraph regardless of author.** If you can't explain it in Q&A you're graded as not understanding it. **A "black box" excuse ("the AI suggested this") is not an acceptable engineering justification.**
3. **No AI-authored deliverables** — generating complete code or copying from a prompt = **zero**; primarily "AI-authored" report/app = zero + possible disciplinary action.

**Quality claim:** *"It's very good with UI. It's very bad with backend code. It does not understand quality."*
**Required workflow:** refactor → peer review before the default branch → return to developer if quality is low.
**Why it bites:** code quality feeds the **holistic** score, so it drags the whole project mark, not just its own 15.

---
**Learning outcomes:** understand Agile/Lean fundamentals; apply them to a real project; demonstrate effective stakeholder communication; demonstrate good project planning and management; critically reflect on practical experience.
