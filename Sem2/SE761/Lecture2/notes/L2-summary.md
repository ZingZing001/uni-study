---
course: SE761
lecture: 2
type: summary
title: L2 one-page summary — rationale, purpose, justification; says/wants/needs
tags: [se761, revision, cram]
---

# ⚡ SOFTENG 761 L2 — one-page summary

> [!warning] No slide deck exists for this lecture
> Transcript is primary; the three **Canvas pages** carry the precise wording. Quoted Canvas wording is marked **(C)**.

## 🔭 The pipeline

Project description = *"just an idea"*, *"one seed"* — **not** a spec. Not an intro-programming one-liner; you must deliver *"a full software product which must be working and of high quality."*

**Go UP to the rationale. Go DOWN to the justification.** Purpose sits closest to the description.

> **"Do not directly jump to what needs to be built."** Stay at rationale level until *"fully convinced."*

## 🪜 Rationale

**(C)** *"The rationale explains the **broader context and underlying need** that gives rise to the project."*
Spoken: *"a way to get to **the root of the things**… a goal or a motivation."*

**Two generating questions** — and they may appear at **any position** in the list:

| | Asks |
|---|---|
| **So what?** | *"What difference is it going to make? Why is it important?"* |
| **Who cares?** | *"Who is this going to help or affect"* — the **ultimate beneficiaries** (environment · people · community · industry) |

**Three constraints:**
1. ❌ **Never mention the product or solution** — *"none of the points must talk about the product"* ← most-emphasised rule in the lecture
2. ↕️ **Flow high → low**, each point **feeding** the next
3. ✏️ **One sentence per bullet**, ~8–10 bullets

**Ice-cap ladder:** planet → climate change → global warming → communities / human life → …
**Read-out example:** top = *"technology is becoming increasingly pervasive in many aspects of society"*; bottom = *"it is therefore important to build people's confidence in engaging with technology to improve their way of life."*
→ **Product description never revealed. That's the proof it was written correctly.**

> [!success] ✅ Term confirmed — **"speed rationales"**
> Resolved 2026-07-30 against the Assignment 1 brief, which prints **"Speed Rationales"** as a section heading. Low-evidence, from current knowledge only, **no literature review**. "Seed rationales" was a mis-hearing — safe to use the real term in writing.

## 🎯 Purpose

**(C)** *"The **specific goal or intent** of the project **within that larger context**."*
Asserts a **relationship** between the why and the product: *"they must have a relationship which you can present as a purpose."*

> [!important] Proportionality — where marks are lost
> **"You cannot say that by building that product, I will be able to solve the global warming problem. It can contribute a little bit."** Usually *"a very minute bit of the overall solution."*
> **Claim contribution, never solution.**

Closest artefact to the client's description: *"when you read your allocated project description, you are basically looking at the purpose."*

**(C) Example:** develop a mobile app letting individuals and small businesses share surplus food in real-time, **thereby** reducing food waste and supporting local food security.
= **what is built** + **what it contributes to**, joined by *thereby*.

## ⚖️ Justification

**(C)** *"Why this solution is **feasible and valuable**, often referring to **evidence, demand, or practicality**."*

Assessed against **team · budget · time · other resources — in communication with the client**. Verdict: feasible or not.
**Also known as the business case.** ← memorise
Comparable products count: *"the solution has worked for other competitors, a similar solution might work for them as well."*

**(C) Example stacks three evidence types:** competitor precedent + stakeholder demand signal + practicality (accessible, scalable, cost-effective).

## 🗣 Says → Wants → Needs

**(C)** *"It's common for what a client says, wants, and needs to differ due to **unclear communication, evolving understanding, or unspoken assumptions**."*
Spoken: *"we all are human beings, and **what we say might not reflect what we actually want**."*

| | What it is | Source | Tell |
|---|---|---|---|
| **Says** | Literal words / the description. Vague. | handed to you | **quoted**, "describes" |
| **Wants** | Initial expectation, unstated | discussion / questions | **"envision"**, **"imagine"** |
| **Needs** | Real business requirement after constraints | analysis / research | **emerges from analysis** |

**Fitness studio (C):**
- **Says** — *"We need a calendar where users can book a class with one click."*
- **Wants** — appealing calendar, instant booking, Google Calendar integration, mobile responsive, drag-and-drop
- **Needs** — view classes · check availability · book/reserve · confirmation — **plus** capacity management · preventing double bookings · payment integration · cancellations and waitlisting

> [!important] The asymmetry is the point
> Decorative wants **dropped**; four operational requirements the client **never mentioned appeared**. The journey is subtractive *and* additive — and the additions are what sink a project if missed.

**Endpoint:** needs = **the product backlog in Scrum**. *"You start with says and then get to product backlog, which is the actual needs."*
→ joins to **L1-C06**: the Spike (Sprint 1) is where the backlog gets compiled.

**Collapse case:** if the client is technical, says/wants/needs may coincide — **you still hold the discussions to confirm**.
**Transport analogy:** says *"fly to my office"* → wants an aircraft → needs **a bike** (office is nearby).

## ❓ Ask WHY first

*"Why does this matter? Who are the affected parties, stakeholders, users?"*

> [!important] Dual benefit
> Extracts detail **and** *"gives an impression to the client that you are **more interested** in developing the project."*

Feels rude; do it anyway — *"that is the first core question."*
**Before the meeting:** infer a rationale and **write it down** · **no research** · plus a written **sequence of questions**.
Analogy: *"in a class, if the students do not ask questions, they won't learn… **now you are on the other side**."*

## 🪞 Reference-product origin

Non-technical clients' descriptions usually come from **a competitor's or colleague's product they've seen**.
**Ask:** *"Is this description your own idea, or is it coming from somewhere else?"* — *"the more transparent you are, the more correct information you will get."*
**Conflict:** inherited technology stack doesn't suit the requested functionality → **counter-question the client.**
Course clients are *"mostly non-technical"*, so this is the **default case**.

## 👥 Client / product owner / user

PO = *"a representative of the client that will be handling or monitoring the project development… building that communication between the client and the team."*
**In this course: client = product owner.**
⚠️ **L1-C04 is the fuller treatment** — non-technical POs, translation duty, and the **never-stop rule**. Merge these when Scrum roles are formally taught.

## 🔍 Word precision

*"Each and every word has a meaning clear in your mind."*
**accessible** = accessible to everyone · **scalable** = can scale if more users · **cost-effective** = its own claim.
Also a marking criterion — language faults are penalised.

## 🤖 Gen AI drafting (beehive demo)

Demo project chosen *"because it has a **limited description**"* → more scope for rationale work.

**First output failed three ways:** not bullets · not one-liners · **talked about the product**.

| Round | Correction | Rule enforced |
|---|---|---|
| 1 | bigger-picture vision only; global/community impact | so what + who cares |
| 2 | no implementation detail | no solution content |
| 3 | bullet points | format |
| 4 | remove project mentions | **still leaked after round 2** |
| 5 | ensure proper flow | connectedness |

> [!important] The check you can steal
> Flow correction pushed the top rung up from *"pollinators like bees are vital"* to **"a healthy planet depends on stability of ecosystems and biodiversity."**
> **Enforcing flow finds the true top of the ladder.** If the flow feels forced at the top, there's another rung above it.

*"The prompt sequence **is** the manual method."*

**Ownership rule:** *"you need to **own what you submit**… you cannot say that AI gave me this and hence hands off."* Read it fully and justify it in your own mind before submitting.
→ Stated far more sharply in **L1-C10**: *a "black box" excuse is not an acceptable engineering justification.*

---
**Not covered:** **Agile**, **Scrum and Kanban** — both listed on the Canvas contents page, both deferred to the following week.
