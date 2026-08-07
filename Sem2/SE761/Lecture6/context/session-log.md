# SE761 Lecture 6 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-08-07 - Mode A ingest - device: macbook
Covered: full ingest of Lecture 6 (Assignment 3 and the evidence-backed rationale). Transcript only, no deck. Wrote L6-notes.md (10 concepts), L6-summary.md, L6-flashcards.tsv (64 cards, validated). No figures - nothing to rasterise.

This is **the last formal lecture of SE761**. From here it is project work: sprint 1 presents in week 6, final presentation week 11, roughly eight weeks of development in between, and the mid-semester break flagged as important.

The whole lecture is one thing: **Assignment 3 is Assignment 1 done properly.** Same rationale skill, now on your allocated project, split by theme across the team, and backed by a real research paper. What makes it worth a full note rather than a brief summary is that the lecturer states the *reason* for the odd rules, and the reason reframes the assignment.

**A3 is a credibility exercise for the first Product Owner meeting that happens to be marked.** "So that when you go and meet your clients, your Product Owner, you can present them with that evidence and show them that you know about the thing... so that they have more confidence in your team." Once you read it that way, the standard he gives makes sense: **"Each point that you present must have backing evidence."**

The three client scenarios (C09) are the most transferable content in the lecture, and they are all the same move: research lets you say something to a client that would otherwise be rude or unsupportable. Similar apps already exist - "now, you need to be honest... you might not be knowing about this." A requirement may not be feasible. And the sharpest one, from a live project asking to migrate MongoDB to MySQL: "Is this understanding presented by the Product Owner correct or not? It might be outdated." That is **L2-C05's says/wants/needs with citations attached** - research is how you get from *says* to *needs* before you have even met them.

Two rules worth not getting wrong. **The paper eligibility rule** is length-based (5 pages double-column, 8 single, references excluded) and it exists to exclude "idea papers" - it is a proxy for having enough method and result to reflect on. And **the both-anchors rule** for the four questions: every answer must be relevant to *both the paper and your project*; a general answer scores nothing. That is the same failure mode A2 warns about, arriving from the opposite direction.

The theme-decomposition worked example is genuinely reusable. Five themes out of the smart-home AR project, and they follow a pattern - core technologies, then a quality attribute (usability/accessibility), then an enabling technology, then integration. Worth trying that template against any build project.

One correction to a natural assumption: with eight people and maybe three themes, **the binding constraint is one unique paper per person, not one theme per person.**

Also captured the A1 marking feedback the lecturer volunteered to the class - some submissions mentioned the solution when the brief prohibited it - and the fact that this becomes *permissible* in A3, where **purpose** may be brought in. That boundary shift is recorded in both this note and the A1 retrospective.

Source quality is fair. The A3 walkthrough is intact; the last third is workshop cross-talk about individual projects and has mostly been discarded.

Quiz: none. All 10 concepts untested, scheduled 2026-08-08.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **Get A3's due date** - never stated in this lecture. Also fetch the **A3 brief PDF** from Canvas Modules 1 & 2; only A1.pdf and A2.pdf are in the repo.
3. Ask what **"agility reflection"** means as an A3 rubric criterion, and how the remaining 3 marks split.
4. When quizzing L6: lead with **C09** (the evidence standard and the three client scenarios), **C07** (the both-anchors rule), **C06** (paper eligibility and why idea papers are excluded), **C04** (eight people, three themes - what actually binds).
5. **The retrieval debt is now the whole story for this course.** SE761 has L1-L6 ingested, 66 concepts, and zero quiz attempts. Next session should be Mode B, interleaving across all six lectures.
