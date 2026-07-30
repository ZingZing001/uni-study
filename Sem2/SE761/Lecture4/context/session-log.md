# SOFTENG 761 Lecture 4 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-07-30 - Mode A ingest - device: macbook
Covered: full ingest of Lecture 4 (Wed 29 Jul, the paper-plane Scrum simulation). Wrote L4-notes.md (12 concepts, L4-C01 to L4-C12), L4-summary.md, and L4-flashcards.tsv (62 atomic cards, validated exactly one tab per line). Ingested in the same session as Lecture 3.

**The judgement call this lecture forced.** It is a workshop, not a lecture - two hours of a game with almost no declarative content. The temptation was to treat the whole thing as noise and keep only the Assignment 2 brief. That would have been wrong. The teaching content is not the rules of the game; it is the **debrief**, where the lecturer names each failure the class produced and generalises it. So the filter applied was: the game's mechanics are a teaching device and are recorded only where a concept depends on them (the story-point mapping, the acceptance criteria, the sprint 1 results table); every generalisation drawn from them is signal and got a concept ID.

The strongest thing here is that **every failure mode the class hit is one L3 explicitly warned about**, and they hit them anyway under a five-minute timebox. Team C forgot an acceptance criterion that all three members had heard. Nobody built a realistic test rig despite being told they could test anywhere. Two teams carried competing designs after agreeing which was better. That gap - knowing the rule and breaking it under pressure - is the actual content, and it is what Assignment 2 asks the student to reflect on. The notes cross-link each L4 concept to the L3 concept it instantiates, so the pairing is visible rather than implied.

Two places where I did NOT smooth over a problem in the source:
- **Sprint 2's numbers.** Only Team D's 5->6 survives the crosstalk cleanly. Team A has two mutually inconsistent statements - the PO says "you got it, as you promised" at the review, and the debrief says "the difference between estimated and actual is still there". Rather than pick one, both are recorded and the notes say plainly that no number should be cited for Team A. The sprint 2 table is a collapsed block with explicit gap markers.
- **The sprint-length rule.** He states "we never alter the sprint lengths" and then alters the planning and execution timeboxes in both directions. That is not a contradiction - the sprint boundary is the invariant and internal events are timeboxed for focus - but it needed saying rather than quietly reconciling, so L4-C03 makes the distinction explicit and notes that the two sprints are therefore not strictly comparable.

Signal/noise: the entire Assignment 2 brief went to admin-and-dates.md, and it is substantial - three-paragraph structure, 800-900 words, how many project examples are required, the rubric, and the two named fail conditions (confusing values with Scrum implementation; writing in non-reflective language). One thing worth flagging loudly and now recorded in that file: **Assignment 2 forbids Gen AI outright**, reversing Assignment 1's policy where AI use was permitted and worth 2 marks with a declaration. Carrying the A1 habit into A2 would be a real, avoidable loss.

Kept as signal rather than admin: the PO's admission of his own two process mistakes (no restriction on building during planning; no spare paper for testing). It looks like housekeeping but it carries a transferable claim - a retrospective's target is the whole system, including how the customer runs the engagement, not only the team's behaviour. That became L4-C12.

Transcript quality is poor, the worst so far, and the failure is characteristic of a workshop: the lecturer's framed segments are intact while the room noise ate most student contributions. Confirmed garbles are tabulated in admin-and-dates.md; the useful ones are "it's fun" for "it spun" (the no-spin criterion failing, which appears repeatedly during flight tests) and "athletics" for "aesthetics".

Quiz: none. All 12 concepts are notes-written-untested, scheduled for first retrieval 2026-07-31.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **Assignment 2 is due Friday 7 August** and is the near-term priority. It needs L3 for content and L4 for lived experience. The most useful next session is not a quiz - it is working through the reflection's structure and checking the draft against the two named fail conditions in `admin-and-dates.md`. Note the ban on Gen AI: help with understanding and critique of the student's own attempt only, never drafting.
3. After that, Mode B. SE761 now has **45 untested concepts** (L1 10, L2 10, L3 13, L4 12) and nothing has ever been quizzed. Stop ingesting.
4. When quizzing L4, prefer Apply/Analyse framings - every concept here has a concrete failure attached, so "team X did Y, diagnose it" works far better than "define Z". Priorities: C02, C05, C06, C10, C11.
5. Predictable misconceptions to watch for: reading Team D as the winner because they built the most; treating an estimate as an ambition rather than a prediction; diagnosing Team C's forgotten logo as carelessness rather than a structural inspection failure; putting the retrospective after planning.
