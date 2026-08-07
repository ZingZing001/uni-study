# ENGGEN403 Lecture 5 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-08-07 - Mode A ingest - device: macbook
Covered: full ingest of Lecture 5 (social cost benefit analysis), Marc Lewis. 40-page deck plus transcript, both good quality. Wrote L5-notes.md (14 concepts), L5-summary.md, L5-flashcards.tsv (123 cards, validated). Twelve figures exported.

This lecture is the **financial case** from L4, and it is unusually concrete: seven named Treasury steps, a fixed discount rate, a named database, and a fully worked exemplar. Almost none of it is arguable, which makes it the most directly examinable lecture so far.

Three things carry the most weight.

**The counterfactual (C05).** The bridge-over-river example does the whole job in five lines: a bridge costing $20 m and saving $25 m has an NPV of +$5 m against "no bridge, no ferry", and −$5 m once you notice a private ferry would otherwise have started. Same bridge, same costs, reversed conclusion. Paired with the two readings of do-nothing - "do nothing more" (BAU) versus "do less" (roll back) - this is the single highest-leverage idea in the lecture, and the transcript only gestured at it. The slide has the numbers.

**The VoSL definition (C07).** $12.5 M NZD, and the slide is unusually careful: *not* the value of an identifiable person's life, but "an economic measure of how much society is willing to pay for small reductions in mortality risk across a population". That precise phrasing is the sort of thing that gets marked, and it is easy to paraphrase into something wrong. What makes it click is the pairing: convenience already has a price ($36.18/hr to not sit in congestion), so without a VoSL figure, safety loses by default. The Royal Oak roundabout is the case - 2018 recommendation not implemented, 2022 cyclist killed.

**The worked monetisation (C10).** Slide 29 is the appendix template: lettered assumptions each with a citation, arithmetic shown line by line, a rounded bold headline. Three blocks - wellbeing (0.05 life-satisfaction points x $5,212/point x 5,330,600 people = $1.4 bn/yr, 10 yrs at 8% = −$12 bn), marine life (380,000 t x 0.5% x USD $15,000 x 1.73 = ~$50 m), and littering (8.3% ÷ 14.5% x $14 x 2.02 m households = $16.2 m/yr). The magnitudes are the lesson: a $12 bn hole and a $16 m/yr patch. Slide 29 says it outright - "sometimes the best option is simply the least bad (smallest negative NPV)".

Two corrections the slides forced against the transcript: monetise **1-3** primary impacts, not the "2 to 5" said aloud; and the pre-COVID VoSL was **$4.53 m**, not the "around $5 million" in the audio.

The most quietly important line in the deck is on slide 30: CBAx "gives exact dollar values, estimation unlikely to be that accurate (IMPORTANT FOR SYSTEMS WEEK)". It is the same idea as L4's 17-versus-16 critique, arriving from the opposite direction - there, a made-up score pretending to be evidence; here, a real number pretending to be precise.

Quiz: none. All 14 concepts untested, scheduled 2026-08-08.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. Ask what **timeframe of analysis** the course requires. The lecturer promised it and never gave it; the exemplar uses 10 years throughout.
3. When quizzing L5: lead with **C05** (bridge/ferry - can the counterfactual be reversed?), **C07** (state the VoSL definition, not a paraphrase), **C10** (walk a calculation end to end), **C09** (why the assumptions beat the number). C13's "intangibles MUST be highlighted in the summary" is a cheap mark that is easy to forget.
4. **The retrieval debt is the real problem**: this course has L1-L5 fully ingested and zero quiz attempts. Next session should be Mode B.
