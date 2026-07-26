# SOFTENG 761 Lecture 2 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-07-27 - Mode A ingest - device: windows-desktop
Covered: full ingest of Lecture 2 ("week one, lecture two"). Wrote L2-notes.md (10 concepts, L2-C01 to L2-C10), L2-summary.md, and L2-flashcards.tsv (57 atomic cards, validated one tab per line).

Unusual source situation. There is NO slide deck for this lecture - confirmed by the user, who also pointed out that the lecture is essentially a walkthrough of the Canvas pages under Modules 1 & 2. So the normal hierarchy inverted: the 452-line auto-generated transcript is primary for reasoning and emphasis, and the three fetched Canvas pages carry the precise wording that gets marked. Both recorded where they differ. Canvas pages were fetched through the user's existing browser session; no credentials were involved.

Signal/noise: Assignment 1 dominates the back half of the lecture and all of it went to admin-and-dates.md - due date, 15 marks / 3%, quiz-format submission, 200-word limit, marking rubric, late penalties, and the Gen AI declaration policy. Kept as signal: the ownership principle behind the AI policy (L2-C10), because it is a transferable rule rather than a course mechanic. The project catalogue zip is reference material for project selection only - explicitly not quizzable, no concept IDs drawn from it.

Quiz: none yet. All 10 concepts are notes-written-untested, scheduled for first retrieval 2026-07-28.

Transcript quality is fair, not good, and that matters here:
- The low-evidence rationales are rendered "speed rationales". Given the lecturer's earlier "one seed" framing, "seed rationales" is equally plausible. NOT resolved - flagged in open_questions and admin-and-dates.md. Do not use either term in writing until confirmed.
- The staff member handling project organisation appears as Razer / Reza / Risa / Arisa. Probably all Reza.
- The transport analogy renders the middle term as "a R", almost certainly "a car".
- Assignment 1 rubric as spoken totals 12 + 2 = 14 against a stated 15.

Also noted: the Canvas "Contents of Module 1 and 2" page lists three topics - From Idea to Rationale, Agile, Scrum and Kanban - but only the first was taught. The other two were deferred, so Modules 1 & 2 are not fully covered by this lecture.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. 10 items due 2026-07-28, all L2, all never tested. Interleave with ENGGEN403 L1 items, which are also outstanding.
3. Run a Mode B quiz round on L2. Prioritise C02, C03, C05 - they are high priority and carry Assignment 1. Predictable misconceptions to watch for: mentioning the product inside a rationale bullet (the single most-emphasised rule), overclaiming in the purpose (solving vs contributing), and treating "wants" as the destination rather than the midpoint.
4. SE761 Lecture 1 is un-ingested and has both a deck (00-Agile_Course_Introduction.pdf) and a transcript. Do that next - it is out of order right now.
5. Expect Agile / Scrum / Kanban in Lecture 3; L2-C08 (client vs product owner) is preliminary and should be merged into the fuller Scrum roles when they arrive.

---

### 2026-07-27 - refinement pass (Obsidian + diagrams) - device: windows-desktop
Covered: rewrote L2-notes.md and L2-summary.md to the standard added to CLAUDE.md sections 3.3a and 3.3b. No new source material was read; the concept set is unchanged at 10, and the 57 flashcards were already atomic and were left alone.

**On visuals - the honest position.** This lecture has no slide deck, so there is nothing to rasterise. I tried to re-check the three Canvas pages for embedded images or diagrams, but the browser extension dropped out before the check completed. From the text captured on 2026-07-26 those pages are plain prose with no figures. So every diagram in the refined notes is **generated, not sourced** - which section 3.3a permits only where the source has no figure for that relationship. Each is labelled as mine at the top of the file so they do not get reproduced in an assessment as course material. Four were added: the up/down pipeline, the says-wants-needs journey terminating in the product backlog, the reference-product technology conflict, and the Gen AI correction sequence mapped onto the rationale rules.

**Structural changes.** YAML frontmatter; callouts throughout (abstract / question / quote / example / important / warning / bug); collapsible blocks for the long reference material - the full fitness-studio walkthrough, the five Canvas quiz classifications, and the self-test; tables for every contrast that was previously parallel prose; a revision-order hint at the top; and internal links.

**Cross-lecture links added.** Three that matter and were previously invisible:
- L2-C05 (needs become the product backlog) now links to L1-C06 (the Spike is where the backlog is compiled). Those two halves were sitting in separate files saying complementary things.
- L2-C08 now carries an explicit warning that L1-C04 is the fuller treatment of client vs product owner, rather than leaving two half-answers.
- L2-C10 (ownership rule) now points at L1-C10 pillar 2, which states the same principle far more sharply.

The unresolved "speed rationales" vs "seed rationales" term was promoted from a footnote to a bug callout in both files, since it is the one thing here that could actively mislead if written into an assignment.

Quiz: still none. All 10 concepts remain untested.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. Nothing was learned or tested in this pass - it was presentation only. The 51-concept untested backlog is unchanged.
3. Next session should be Mode B. For this lecture prioritise C02, C03, C05.
4. If the browser extension is working, re-check the three Canvas pages under Modules 1 & 2 for embedded images; if any exist they should be pulled into notes/figures/ and the generated diagrams demoted.
