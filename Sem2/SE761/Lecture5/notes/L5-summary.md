---
course: SE761
lecture: 5
type: summary
title: L5 one-page summary — reflection models and teamwork risks
tags: [se761, revision, cram]
---

# ⚡ SE761 L5 — one-page summary

## 🔍 Reflection

> **"Reflection is the conscious exploration of an experience. In order to learn from an experience, you need to reflect on it."**

**Learn from the past → apply in the present → better future.** It's an **agile** obligation, not a study skill: *"one of the most important principles of agile software development… we keep on focusing on improving our development steps and the overall process."* → L3-C03 principle 12, L3-C10 **adaptation**.

A **structure** helps because it moves you out of **"auto-pilot"**; most models are drawn as **cycles**. Unstructured reflection mostly doesn't happen — *"if the traffic light goes yellow… how many of us actually reflect on this after reaching home?"*

## 🔄 Gibbs' reflective cycle ⭐

**Description** (what happened?) → **Feelings** (what were you thinking and feeling?) → **Evaluation** (what was good and bad?) → ⭐ **Analysis** (what sense can you make of it?) → **Conclusion** (what else could you have done?) → **Action plan** (if it arose again, what would you do?)

**Analysis cue questions:** what sense can you make · ⭐ **how do past experiences compare to this?** · **how does theory or evidence fit with this?** · how did your involvement affect the outcome?

> ⭐ **"That analysis part is what is being asked in assignment two."** — and *"how do past experiences compare to this?"* is the A2 3-mark rubric line almost verbatim.

Educational origin; best for **everyday situations**. Don't drop the other stages — feelings and evaluation still belong.

## 🧭 Johns' model of structured reflection

**Describe the experience → Reflection → Influencing factors → Could I have dealt with it better? → Learning**

⭐ **Look inwards** (your thoughts and feelings) **and look outwards** (the incident, your actions, **whether they were ethical**, external factors). Nursing origin. Asks *"how did the other person feel?"* and *"did I act for the best?"*

**Four ways of knowing:** empirics (scientific) · **ethics** (moral) · personal (self-awareness) · aesthetics (the art of what we do).

Also recommends **involving a mentor** — reflection with someone else is more powerful.

**The ethics example:** your team has accepted a complex piece of code that could be simplified. *"The biggest factor is time, and you have to go with your team."* Energy efficiency → CPU → **carbon footprint**. *"Try to make genuine decisions in those situations."*

## ♻️ Kolb's learning cycle

**Doing it** (concrete experience) → **Reflecting on the experience** (reflective observation) → **Making sense** (abstract conceptualisation) → **Planning what to do** (active experimentation). **Enter at any stage**; it's a **spiral**.

⭐ **Distinguishing move: drawing generalisations.** Compare good experiences across projects; if they held both times, generalise. And they can be **falsified** — *"the good experiences might turn into bad experiences, and so they won't be generalisations anymore."*

**Software design patterns are generalised experience** — solutions that generated good outcomes often enough to get a name. Where a pattern doesn't fit, *"this generalisation doesn't work in my situation."*

## ❓ Rolfe, Freshwater & Jasper

**What? → So what? → Now what?**
**What** = description (my role, what I was trying to achieve, actions, response of others, consequences, feelings). **So what** = understanding (what does this tell me about me/others/my attitudes; what did I base my actions on; what other knowledge can I bring). **Now what** = improvement (what do I need to do; what broader issues; **what might be the consequences of this action**).

Novice-to-expert scalable. ⚠ **"So what?"** is L2-C02's rationale test arriving from another discipline.

## 🎛 Choosing

1. **You need not use one** — *"we are not going to mark you against these models."*
2. **If you use one, name it in the submission.**
3. **Hybrids explicitly allowed** — *"pick a few things from this model, a few things from that model."*

They converge: *"all the models will have a step that asks you to think about the past, and then apply that knowledge in future."*

| **Gibbs** | closest fit to the A2 rubric |
| **Johns** | your experience turned on a **decision** |
| **Kolb** | you have **more than one** past project |
| **Rolfe** | you're short on time |

## 🔁 Reflection inside Scrum

Team reflection lives in the **sprint retrospective** and **sprint planning**. But *"you will be expected to keep on doing **individual reflection** as you go."*

⭐ **Retrospective = process. Review = product** (the demo to the Product Owner). Teamwork risks belong in the **retrospective** (quiz Q20).

## ⚡ Extreme Programming

**~10–15 good development practices**: TDD, pair programming, continuous integration, refactoring.

⭐ **Why "extreme":** *"whatever good practices are implemented in traditional software development methodologies, we use them — and we use them in an **extreme manner**."* Code review every sprint → **pair programming**, i.e. review continuously. *"So that means it is a kind of continuous reflection as well."*

## ⚠️ The 15 teamwork risks

1 **Uneven Workload Distribution** ("free riders"; burnout and resentment) · 2 **Poor Communication** · 3 **Lack of Role Clarity** · 4 **Conflicting Schedules** · 5 **Inconsistent Skill Levels** · 6 **Decision-Making Conflicts** · 7 **Lack of Commitment / Motivation** · 8 **Version Control & Code Integration** · 9 **Scope Creep** · 10 **Ineffective Project Planning** · 11 **Lack of Leadership** · 12 **Dependency on Key Members** · 13 **Cultural or Personality Clashes** · 14 **Inadequate Testing & QA** · 15 **Poor Documentation**

⭐ **#2 poor communication is "the most common cause of risks becoming issues"** — stated since lecture one.
⭐ **Unrealistic estimates (#10):** *"pick a deadline slightly later than what you would generally think is achievable."*
⚠ **Volunteering for more work is also a risk** — *"it leads to burnout."*
⚠ **One-week sprints make non-responsiveness fatal.** *"The first thing you must ensure is that you are reachable."*
⭐ **Risk identification is everyone's job — "not a responsibility of the Scrum Master."** First action is always **talk to them**.

Also: don't start work until your role is clear · don't hide your availability · decision conflicts are a **positive** signal but **never take it to the personal level** · keep a visual on repo pushes (scope creep) · *"there should still be a sense of leadership in each member"* · documentation must be understood by everyone **at equal levels, in the same manner**.

## 🛠 Risk → mitigation mapping

| ID | Risk | Impact | Likelihood | Priority | Mitigation |
|---|---|---|---|---|---|
| R1 | Uneven Workload | High | Med | High | Define roles early, task tracking tools |
| **R2** | **Poor Communication** | **High** | **High** | **High** | **Regular meetings + comms tool (Slack, Teams)** |
| R3 | Lack of Role Clarity | Med | High | High | **Document responsibilities in a Team Charter** |
| R4 | Conflicting Schedules | Med | High | Med | Shared calendars; fixed weekly syncs |
| R5 | Inconsistent Skill Levels | Med | Med | Med | Pair programming & knowledge sharing |
| R6 | Decision-Making Conflicts | High | Med | High | **Voting mechanism; assign final authority** |
| R7 | Lack of Commitment | High | Med | High | Peer evaluations; celebrate milestones |
| R8 | Version Control Issues | High | Med | High | Mandatory Git training; **daily commits** |
| R9 | Scope Creep | High | Med | High | **Freeze scope early; maintain change log** |
| R10 | Ineffective Planning | High | Med | High | Agile sprints; define deliverables weekly |
| R11 | Lack of Leadership | High | Med | High | **Rotate leadership roles per milestone** |
| R12 | Dependency on Key Members | High | Med | High | **Cross-train on critical tasks** |
| R13 | Cultural/Personality Clashes | Med | Med | Med | Team bonding; conflict resolution process |
| R14 | Inadequate Testing & QA | High | Med | High | **Testing tasks in sprint planning; assign QA roles** |
| R15 | Poor Documentation | Med | High | High | **Documentation checkpoints per sprint** |

⭐ **R2 is the only High/High.** Only R4, R5, R13 are Medium priority. R1 vs R3: one is a **tool** fix, one is a **document** (Team Charter) fix.

**Voting mechanism = planning poker**, described without the name: flash cards with point values, revealed together, Scrum Master **gently facilitates**, discuss variation *"until they get to one specific estimate."*
**Celebrate milestones** — *"throw a party after sprint one… but do not spend the whole next week partying."*
**Pick one platform** — Discord vs Slack vs email is R13 in practice.

## 🚦 Risks vs issues ⭐

> **"As long as you have not started things, they are risks… then there is a potential that they will be converted into real issues."**
> **Risks are mitigated. Issues are resolved.**

The real danger: *"there would be a tendency to **not look at a certain situation as a risk when it is actually a risk**."*

**`Project_Risk_Quiz.pdf`** — 20 questions, **not a Canvas quiz**, not assessed. Answers given: Q1 B · Q2 C · Q3 C · Q4 A · Q5 B · Q6 B · Q7 D · Q8 C · Q9 B · Q10 A · Q11 B · Q12 C · Q13 B · **Q20 C (sprint retrospective)**. Q14–Q19 left to you.

## 👤 People (not examinable)

**Ken Schwaber** and **Jeff Sutherland** — Agile Manifesto authors, **invented Scrum**. **Martin Fowler** — code smells, refactoring. **Robert C. Martin ("Uncle Bob")** — *Clean Code*. **Taiichi Ohno** (Toyota) — **Kanban**, 1950s. **David Anderson** — applied Kanban to software.

**Quotes:** *"By the end of the sprint you must have a working product."* · ⭐ *"If you adopt only one agile practice, let it be retrospectives"* — **"if you are not doing retrospectives, you are not doing agile at all."** · *"Continuous improvement is better than delayed perfection."* · *"Agile is an attitude, not a technique with boundaries."* · *"The best way to get a project done faster is to start sooner. And the only way to go fast is to go well."* · *"It doesn't matter how good you are today — if you're not better next month, you are no longer agile."*
