---
course: SE761
type: assignment-plan
assignment: 3
title: A3 — writing skeleton
date: 2026-08-14
status: drafting
tags: [se761, assignment, reflection, plan]
---

# A3 — writing skeleton

**Paper:** Tham, Brady, Ziefle & Dinsmore (2025), *Barriers and Facilitators to Older Adults' Acceptance of Camera-Based Active and Assisted Living Technologies: A Scoping Review*, Innovation in Aging 9(2). 50 studies, TDF-mapped, 28 barriers / 19 facilitators.

**Target: 880–900 words.** Four content questions, each its own paragraph, each visibly grounded in the paper.

> [!warning] Rationale, not solution
> No React, no CARE server, no API design, no architecture. Write about people, adherence, acceptance and trust.

---

## The link that makes this paper unmistakably relevant

Our agent performs a **mandatory visual ID check** on the patient — the PO called it non-negotiable. That means **a camera, in an older person's home, pointed at them.** The PO believes he sidestepped surveillance by choosing a trust-based self-report model, and in the sense he meant, he did: nothing verifies the pill was swallowed. But a camera is still present in the deployment.

So a review of what makes older adults accept or reject **camera-based** in-home technology is not adjacent to our project. It is directly about a component we have already committed to.

Use this as the spine. It gives every section something concrete to attach to.

---

## ¶1 — Opening (~90 words)

- Name the paper and what it is (scoping review, 50 studies).
- State the lens: **human acceptance**, distinct from the capability-and-usability lenses your teammates took.
- One sentence on what you assumed before reading. ← **YOU SUPPLY**

## ¶2 — Why the paper was useful (~150 words)

Findings available:
- Resistance is **negotiable, not fixed**. Privacy is traded for safety when need is perceived. Prior falls, stroke or heart attack sharply raise acceptance.
- Acceptance is not an education or usability problem — *Knowledge* and *Skills* are marginal TDF domains (<3% combined), while *Beliefs about Consequences* carries 33.8%.

Angle: the project description and the PO meeting told you *what* to build and that monitoring was unwelcome. Neither told you that unwillingness is **conditional and movable**, or what moves it.

- What specifically could you not have known without this? ← **YOU SUPPLY**

## ¶3 — What surprised you (~150 words)

The strongest material you have. Pick **one**, develop it properly — do not list all three.

- **The self–other gap.** People deny needing it themselves while enthusiastically endorsing it for others "worse off", deferring their own need to a hypothetical future. **95.5% agreed it would be useful later in life; only 15.5% would use it now.**
- **Preference reversal under imagination.** Participants who rejected cameras in the abstract flipped when asked to picture themselves on the floor after a fall.
- **Privacy framing inverts.** Some saw home cameras as privacy-*enhancing* relative to a care home.

Reflection requirement: name the belief you held **before**, then the finding, then what it did to that belief. Without the "before", this reads as summary and loses the reflection mark. ← **YOU SUPPLY the "before"**

## ¶4 — What the client would value (~170 words)

The most actionable finding for our PO:

- **Control matters more than access.** Choosing who sees the data, when the camera runs, and which rooms it covers was often the *precondition* for acceptance. Motion-triggered-only operation made people feel "less spied on."

Why he'd care: he reasoned from *whether* to monitor. The evidence says the decisive variable is *who controls it*. That reframes a binary decision as a design space — and it does so without contradicting his instinct, which matters when you're telling a client something they didn't ask for.

Second thread if words allow:
- **Existing social support reduced acceptance** (technology seen as redundant), while **fear of burdening caregivers cut both ways** — relevant because the caregiver role is a first-class part of the web page he prioritised.

- Your judgement on whether his trust-based decision holds up ← **YOU SUPPLY**

## ¶5 — How it shapes your perspective and approach (~170 words)

Candidate threads — pick what you actually believe:
- The self–other gap implies our hardest problem may be **adoption, not capability**: the people the system targets are the least likely to accept they need it.
- Acceptance is a **product requirement**, not a deployment afterthought — it belongs in how requirements get elicited.
- Consent, visibility and control are things to raise with the client **early**, while the rationale is still being settled.

- What will you now do or ask differently? ← **YOU SUPPLY**

## ¶6 — Questions for the client (~80 words)

Two or three, each traceable to a finding. Candidates:
- Who is the intended first user — someone who already accepts they need help, or someone whose family decided for them? *(self–other gap)*
- Do patients get any control over when the visual ID check runs, or who sees the interaction history? *(control-as-precondition)*
- Where a patient already has strong family support, does the system risk being seen as redundant? *(existing social support finding)*

- Choose and phrase in your own words ← **YOU SUPPLY**

## ¶7 — ChatGPT reflection (~90 words)

Must include where it was **not** useful. Honest limits earn this mark; universal praise doesn't.

- What you used it for, and what it couldn't do ← **YOU SUPPLY**

---

## Final selection (after Johnson's read — 14 Aug)

Material generated far exceeds 900 words. The task is now **cutting**, not writing. Selection below.

### Keep — load-bearing

| Where | Content |
|---|---|
| Prior | Expected the flat privacy story: older adults reject cameras, privacy is the blocker, therefore route around it with non-visual sensing. Expected the paper to validate the PO. |
| ¶3 Surprise | **Privacy objections are not stable preferences but conditional prices.** Preference reversal (rejected cameras in the abstract → preferred them over pendant alarms when imagining themselves on the floor after a fall); framing inversion (cameras read as privacy-*enhancing* against the alternative of a care home). **Consequence: stated-preference data in this domain measures the frame, not the preference.** |
| ¶3 or ¶4 | **Self–other gap** — 95.5% useful later in life, 15.5% would use it now. An *identity* objection, not a usefulness objection in privacy costume. No feature work touches it. |
| ¶4 Client value | **Acceptance is lowest among the healthy and independent, highest among those with disability, MCI or dementia.** Our stated users are elderly people who forget medication — closer to the segment where the privacy objection is *weakest*. |
| ¶4 Client value | **Control, not access, is the precondition.** Motion-only activation and user-specified times made people feel "less spied on"; identity-redacting filters were "a key precondition to acceptance for many." The middle ground the binary framing ruled out. |
| ¶2 Useful | Resistance is negotiable; TDF weighting shows *Knowledge* and *Skills* marginal (<3%) against *Beliefs about Consequences* at 33.8% — acceptance is not a training or usability problem. |
| ¶5 Perspective | Acceptance is a **requirements** concern, not a deployment afterthought. And the caregiver mitigation spends caregiver goodwill, which the paper lists as a barrier (concern about inundating or burdening carers) — a cost nobody has priced. |
| Quote | One verbatim participant quote — the "granny nap" objection — as evidence of actual reading. One only. |

### Cut — costs marks or words

- **Confidence percentages** (~80%, ~88%, ~92%). Personal analytic style; in a professional academic reflection they read as hedging clutter and consume words the rubric wants spent on substance.
- **"Is the decision stupid?"** — casual register, and the writing-style mark explicitly penalises it.
- **Any meta-commentary about markers, Q&A performance, or what "demonstrates comprehension."** The reflection is the assessment; do not narrate it.
- **The missed-dose surfacing proposal, as a proposal.** See the warning below.
- **The three-products scoping question, as a recommendation to the team.** Keep the underlying insight, drop the internal-process framing.
- Autonomy/stigma paragraph — strong, but overlaps ¶3 and ¶4. Fold one sentence into ¶4 rather than giving it its own paragraph.

> [!warning] The biggest content risk
> The brief says twice: **avoid discussing specifics of the solution you will develop.** The missed-dose-surfacing idea, the "three different products" scoping question, and the Q&A framing are all *solution* content. As written they invite a content deduction.
>
> **Reframe, don't delete.** The defensible version is an insight about how the rationale works, not a feature: *a social mitigation only functions if the person carrying it can perceive the thing being mitigated.* That is a statement about trust-based care models in general, grounded in the paper's caregiver-burden findings — and it stays on the right side of the line. The moment it becomes "we should add X to the caregiver view," it is solution talk.

---

## Before submitting

- [ ] Word count 880–900, counted
- [ ] Each of ¶2–¶5 answers one question unmistakably
- [ ] Every claim traceable to the paper
- [ ] A "before" belief stated at least once
- [ ] No mention of our software solution
- [ ] Paper attached
- [ ] Canvas A3 Quiz, before 9pm
