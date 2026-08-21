---
course: ENGGEN403
type: syllabus-map
tags: [enggen403, index]
---

# ENGGEN403 - Syllabus map

**Fully ingested: Lectures 1-13. 151 concepts tracked, none yet tested.**

## Dependency graph

```mermaid
graph TD
    subgraph W1[Week 1 - framing]
      L1[L1 Mindset, grit, T-shape<br/>12 concepts]
      L2[L2 Systems thinking<br/>9 concepts]
      L3[L3 Science/government interface<br/>10 concepts]
    end
    subgraph W2[Week 2 - the toolkit]
      L4[L4 Business case analysis<br/>13 concepts]
      L5[L5 Social CBA<br/>14 concepts]
      L6[L6 GDP and what metrics miss<br/>13 concepts]
    end
    subgraph W3[Week 3 - back out to the problem]
      L7[L7 Stakeholders at national level<br/>12 concepts]
      L8[L8 Systems thinking and wicked problems<br/>12 concepts]
    end
    L1 -->|problems are interconnected| L2
    L2 -->|wicked problems| L3
    L2 -->|boundaries| L7
    L2 -->|tools deferred| L8
    L3 -->|consensus quadrant| L7
    L3 -->|no clean data| L5
    L4 -->|the financial case| L5
    L4 -->|what you cannot monetise| L6
    L4 -->|steps 2-4 of the methodology| L7
    L5 -->|qualitative impacts| L6
    L6 -->|MCA| L4
    L7 -->|wickedness triangle| L8
    L8 -->|problem statements| L4
    subgraph W45[Weeks 4-5 - delivery]
      L9[L9 Defining and scoping<br/>10 concepts]
      L10[L10 Machinery of government<br/>12 concepts]
      L11[L11 Guest: NEMA<br/>12 concepts]
      L12[L12 Guest: City Rail Link<br/>11 concepts]
      L13[L13 Team project tips<br/>11 concepts]
    end
    L8 -->|causal loops become a procedure| L9
    L9 -->|problem statements| L4
    L6 -->|budget and LSF| L10
    L7 -->|decomposing government| L10
    L10 -->|the slow path| L11
    L3 -->|Whakaari, social licence| L11
    L4 -->|CRL was the opening example| L12
    L9 --> L13
    L10 --> L13
    L13 --> PROJ[Team Project - week 6]
    PROJ --> SW[Systems Week]
    L4 --> SW
```

## Lecture index

| Lecture | Topic | Date | Lecturer | Status | Concepts | Feeds into |
|---|---|---|---|---|---|---|
| 1 | What can ENGGEN 403 do for me? - mindset, grit, T-shaped engineers | 21 Jul | Gerrard | **notes written, untested** | 12 (C01-C12) | goal-setting assignment; the honeycomb frames the whole course |
| 2 | An introduction to systems thinking | 23 Jul | Gerrard | **notes written, untested** | 9 | L3; L8; both projects |
| 3 | Interface of science, engineering and government | 24 Jul | Gerrard | **notes written, untested** | 10 | project framing and messaging; the fishing case is picked up in L7 |
| 4 | Business case analysis and options assessment | 28 Jul | **Lewis** | **notes written, untested** | 13 | the spine of the Systems Week deliverable |
| 5 | Social cost benefit analysis | 30 Jul | **Lewis** | **notes written, untested** | 14 | the financial case |
| 6 | GDP, government spending, and things that metrics miss | 31 Jul | **Lewis + Gerrard** | **notes written, untested** | 13 | the qualitative half of the financial case; MCA |
| 7 | Stakeholders at the national level | 4 Aug | **Di Ienno + Gerrard** | **notes written, untested** | 12 | the strategic case; CSFs |
| 8 | Systems thinking and wicked problems | 6 Aug | **Gerrard + Di Ienno** | **notes written, untested** | 12 | the first morning of Systems Week |
| 9 | Defining and scoping your wicked problem | 7 Aug | **Lewis + Di Ienno** | **notes written, untested** | 10 | causal loops -> problem statements; Systems Week day 1 |
| 10 | Machinery of government | 11 Aug | Gerrard | **notes written, untested** | 12 | who to aim a recommendation at |
| 11 | **Guest: Tom Wilson, NEMA** - advising in the storm | 13 Aug | **Wilson** | **notes written, untested** | 12 | ⚠ compulsory; the emergency counterpart to L10 |
| 12 | **Guest: City Rail Link** - tying it all together | 14 Aug | **Mace + Fenton** | **notes written, untested** | 11 | ⚠ **no deck**; life after the drawings |
| 13 | Putting it all together - team project tips | 18 Aug | **Rachor** | **notes written, untested** | 11 | the Team Project operating manual |

## The through-line

The course builds one argument in three movements.

1. **Weeks 1 (L1-L3) - the framing.** Real problems are not pre-framed, engineering alone will not close them, and you need a growth mindset and grit to stay in the discomfort where learning happens. Those problems have a name (**wicked**), a structure (**elements, interconnections, purpose**) and a critical decision (**the boundary**). The goal is **amelioration, not solution**. And even correct technical work fails without a **values consensus**.

2. **Week 2 (L4-L6) - the toolkit.** Marc Lewis hands over the machinery: the **Better Business Case** framework and options assessment (L4), **social CBA** for what can be monetised (L5), and the **Living Standards Framework, four capitals and MCA** for what cannot (L6). All three are Treasury tools and are designed to interlock.

3. **Week 3 (L7-L8) - back out to the problem.** Stakeholder analysis produces the **critical success factors** that the whole options assessment is scored against (L7), and systems thinking supplies the tools to frame a problem you cannot solve — **iceberg, leverage points, causal loops** (L8).

**L8 closes the loop back to L4**: the pattern layer of the iceberg is where **problem statements** come from, and the strategic case begins there.

4. **Weeks 4-5 (L9-L13) - delivery.** **L9** turns L8's causal loops into a *procedure* ending in a written problem statement. **L10** answers the question every earlier lecture ducked - *when you say "government should", who is that?* **L11** (NEMA) and **L12** (City Rail Link) are guest lectures showing the same machinery under emergency time pressure and under construction reality. **L13** is the Team Project operating manual.

**The arc, in one line:** frame the problem (L1-L3, L8-L9) → cost and compare the options (L4-L6) → find out who decides (L7, L10) → watch it happen for real (L11-L12) → do it yourself (L13 → Team Project → Systems Week).

## Cross-cutting themes

- **Engineering is necessary and insufficient.** L1 (T-shape, "doubling down on more hard sciences will not help"), L2 ("a useful skill set, but not the only skill set"), L3 (the gangs report was technically fine and still failed), and now sourced to the founder of the discipline in L8: **Jay Forrester** — *"the biggest impediment to progress comes, not from the engineering side… but from the management side."*
- ⭐ **"No right answer, only trade-offs" — and the justification is the assessed thing.** Stated three times in one week, by two lecturers, in three different tools:
  - **L4** on the DFV/CSF options matrix: *"It looks great. It's pretty. It tells me absolutely nothing."* A score of 17 vs 16 justifies nothing.
  - **L5** on CBAx: *"Gives exact dollar values, estimation unlikely to be that accurate (IMPORTANT FOR SYSTEMS WEEK)."* Understand the assumptions, not the number.
  - **L6** on MCA against the four capitals: *"Numbers not important, it's the justification behind the numbers."* Choose 17 over 16 without saying why and *"I'll put a big fat zero through your discussion."*
- **Justify both inclusion and exclusion.** L4's named gap in an otherwise strong exemplar; L6's observation that students are strong on positives and weak on negatives and trade-offs.
- **The boundary is the fight.** L2 introduces it, L7 shows it destroying a real project (*"out of scope were all the things that the stakeholders felt strongly about"*), L8 states it as a rule (*"as soon as you've drawn a boundary you're going to have tensions"*).
- **You will not get clean data.** L3-C05 (propagate the uncertainty), L5 (the assumptions behind CBAx figures), L7 (*"you don't know what the unfished volume is… put all those three in an equation and you can back up any argument"*).
- **Amelioration measures create new problems.** Defined in L2 and L8; demonstrated in L5 (plastics do-nothing at -$12 bn against a $16 m/yr recovery) and in L8's school-discipline causal loop (suspension balances one loop and drives another).
- ⭐ **The failure is never the science, it's the translation.** L3 (the gangs report was technically fine and still failed) · L7 (*"put all three unknowns in an equation and you can back up any argument"*) · **L11's bread analogy** (*"with little time or expertise, even the best data doesn't get the opportunity to add value"*) · L12 (*"explain the why, not just the what"*). Four lecturers, four domains, one claim.
- ⭐ **A persistent system works for someone.** L13: *"don't walk into the examination of a system saying it's a mess and broken for everyone - it's probably only broken for some of its stakeholders."* This is the general answer to L9's canvas question *does anyone benefit from the problem as a problem?*, and it explains why interventions meet resistance you never mapped.
- **Rescale the number to the decision-maker.** L5 (timeframe bias and the 8% discount rate) · L10 (election cycles) · ⭐ **L11** (a 1% chance in 50 years becomes **12% in three years, 23% in six** - one and two electoral terms).
- **Check what existing powers already allow.** L7 (EAFM and s9c were already in the Fisheries Act, unused) · ⭐ **L10's regulation ladder** (just do it < regulation change < law change; plastics fitted inside the Waste Minimisation Act 2008).
- **Political values finish the job.** L4 (business cases inform, politics decides), L5 (values or politics *"masquerading as a financial case"*), L6 (wellbeing provisions stripped from the Public Finance Act), L7 (the fisheries portfolio survived a change of government; the transformation plans did not).

## The honeycomb (L1-C12) as the course index

Twelve tiles: **Mindset-Grit** (wk 1) · **Systems Thinking** (wks 1, 3) · **Strategic / Economic / Financial Cases** (wk 2) · **Gov't Context, Management Case** (wk 4) · **Team Building** (wk 5) · **Team Project** (wk 6, dress rehearsal) · **Systems Week** + **McKinsey Workshop** (wk 7) · **Technical Know-How** (from your degree).

By end of L8: mindset/grit, systems thinking, strategic case, economic case and financial case are all covered. Gov't context and the management case are next.

## Terminology to lock down

**Framing:** wicked / complex / long problem · amelioration · elements, interconnections, purpose · emergence · boundary (in scope / out of scope) · consensus quadrant · social licence · T-shaped · grit · SMART-H

**Business case:** Better Business Case (strategic, economic, commercial, financial, management) · indicative → detailed → full implementation · off-ramp · programme business case · DFV · CSF · long list / shortlist / packages · do nothing / minimum / medium / maximum

**Economics:** NPV · BCR · IRR · counterfactual · benefits, disbenefits, costs, cost savings · VoSL ($12.5 M) · willingness to pay · WELLBY · CBAx · 8% discount rate · SOC and SRTP · 2 significant figures · GDP = C + I + G + (X−M) · PPP · productivity (GDP per hour worked)

**Wellbeing:** Living Standards Framework (12 domains, 6 spheres, 4 capitals) · natural / human / social / financial and physical capital · He Ara Waiora (wairua, Te Taiao, Te Ira Tangata; kotahitanga, tikanga, whanaungatanga, manaakitanga, tiakitanga) · MCA (+3 to −3)

**Stakeholders:** power / interest / legitimacy / urgency / attitude · salience (dormant, discretionary, demanding, dominant, dangerous, dependent, definitive, non-stakeholder) · RACI · necessary / nice-to-have / aspirational

**Systems tools:** VUCA · iceberg (events, patterns, structures, mental models) · levels of thinking · Head matrix (tame → very wicked) · twelve leverage points · balancing (B) and reinforcing (R) loops · causal loop diagram · **cluster map · interconnected circle map · problem framing canvas · Cynefin**
**L9:** node polarity (+ / −) · **loop parity rule** (even minuses incl. zero = reinforcing; odd = balancing) · the **problem statement template** (*the problem is ___, which affects ___, because ___, leading to ___*) · **intervention** (not "solution")
**L10:** central vs local · unitary authority · council-controlled organisation · **BIM (briefing for incoming ministers)** · the advice chain (agencies → ministers → cabinet → parliament → agencies) · **baseline vs new funding** · **the regulation ladder** · select committee
**L11:** hazard / exposure / vulnerability / impact / risk · the **four Rs** (reduction, readiness, response, recovery) · **zone of tolerance** · locally led, regionally coordinated, nationally enabled · **maximum credible event** · failure of imagination vs failure of initiative · **relevance / legitimacy / credibility** · the Science Desk
**L12:** **alliance contract** · **Construction Phase Services** · **PS1-PS4** and DC1-DC4 · **ITP** · **hold point vs witness point** · NCR · **DSI** · wider economic benefits · LOD 500
**L13:** **systems research vs scholarly research** · **packages** · lockdown point · cluster map / circle map

## Open across the course

- ⭐ **Nothing has ever been quizzed.** **151 concepts across 13 lectures.** Thirteen consecutive session logs have ended with the same handoff. This is the single outstanding problem with this course.
- ⚠ **L12 has no slide deck.** Both CRL speakers presented throughout; everything is reconstructed from a transcript that badly garbles proper nouns.
- ⚠ **L9's deck is missing ~6 slides**, including the annotated 2024 food-prices causal loop - the only worked example of leverage-point selection in the course.
- **Two full Systems Week exemplar reports** sit unremarked in `Lecture9/resources/` (49 and 56 pages). Nothing in the course walks through a finished report; these are it.
- **The Team Project brief** (released after L13) is not in the repo.
- **Is guest lecture content examinable?** L11 was compulsory; nothing was said either way, and the same question applies to L12.
- **Reading: *Thinking in Systems*, Meadows** — first two chapters minimum, whole book strongly advised, ahead of the team project. Stated in L2 and again in L8.
- **Lecture 10** — machinery of government and budgets, deferred to from both L6 and L7.
- The **timeframe of analysis** for the social CBA was promised in L5 and never given (the exemplar uses 10 years).
- **Commercial fishing** was flagged as deferred in L3 and delivered in full in L7.
- Amanda promised a follow-up walking through past student causal loop examples (L8) — **delivered as L9's live food-prices activity**.
