# ENGGEN403 Lecture 1 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-07-26 - scaffold corrected - device: windows-desktop
No study happened. This folder was created by copying the SE731 placeholder scaffold, so every context file still carried course "SE731", lecture 1, and a stale next_action. Regenerated progress.json / quiz-history.md / admin-and-dates.md / session-log.md with the correct course and lecture and with resources_seen populated from what is actually in resources/.

No notes, no concepts, no quiz yet.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. Nothing is due for review - review-queue.json is empty for this course.
3. Run Mode A ingest for ENGGEN403 Lecture 1.

---

### 2026-07-26 - Mode A ingest - device: windows-desktop
Covered: full ingest of Lecture 1. 25-page deck (text layer present, not scanned) + 378-line auto-generated transcript, quality good. Wrote L1-notes.md (10 concepts, L1-C01 to L1-C10), L1-summary.md, and L1-flashcards.tsv (52 atomic cards, validated one tab per line).

Signal/noise split was the bulk of the work - roughly half this lecture is administration. Everything on assessment weightings, the 27 July goal-setting deadline, the teaching team, lecture times, the SET survey response, the clinic, and Systems Week logistics went to admin-and-dates.md and is not quizzable. Kept as signal: the emphasis-wrapped content (growth mindset and grit are the stated learning outcomes, so both are priority high), and the analogies that carry concepts - the T, the discomfort zone bands, the hope curve. Discarded Kaleb's account of his team's attendance policy as anecdote without a transferable concept; kept the "coherence beats cleverness" student reflection because it states a mechanism.

Quiz: none yet. Interleaved recall (CLAUDE.md section 3.4) did not happen - the user was not present during the ingest, so all 10 concepts are notes-written-untested and every one is scheduled for first retrieval 2026-07-27.

Two flags raised:
- **Diagram gap.** pdftoppm/pdfinfo/pdffonts are not installed on this machine, so slides 17-18 (the course "jigsaw" map), 19, 20, 22 (image-only) and 24 (the success-vs-career graph the lecturer called "my last slide") were never viewed. Notes reconstruct 17-18 and 24 from surrounding text and are marked as such. This is a real hole, not a cosmetic one.
- **Attribution problem.** The marshmallow test was presented alongside the Dunedin study; the paradigm is Mischel's (Stanford). Logged in open_questions and admin-and-dates.md. C06 is priority low partly for this reason - quiz the concept, not the study name.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **10 items due 2026-07-27, all L1, all never tested.** Nothing from other lectures to interleave yet.
3. Run a full quiz round on L1 (Mode B, max 10 questions, Bloom mix: <=2 recall, 4 apply, 4 analyse/evaluate). Prioritise C02, C03, C04, C08, C09 - the high-priority ones. Watch specifically for: treating growth/fixed mindset as a personality type rather than a per-skill continuum, and reading "T-shaped" as generalist. Both are the predictable misconceptions here.
4. Then: install Poppler (`winget install oschwartz10612.Poppler`) and re-ingest the six unviewed diagram pages before starting L2 - L2 is systems thinking, which is diagram-heavy, and going in without a rasteriser would repeat the same hole on worse material.
5. ENGGEN403 L2 and L3 have full resources and are untouched. SE761 has a transcript only (and it is Lecture 2's transcript sitting in the Lecture1 folder) - resolve that before ingesting.

---

### 2026-07-27 - Mode A refinement (diagram pass) - device: windows-desktop
Covered: re-ingest of the six slide pages that the first pass could not see, plus a rewrite of all three note files for Obsidian.

Poppler turned out to be installed all along - v25.07.0 inside a conda env at C:\Users\johns\.conda\envs\environment\Library\bin, just not on PATH. winget reported the package as already present. The earlier "Poppler is missing" conclusion was wrong: only the stripped pdftotext shipped with Git for Windows is on PATH. Recorded in CLAUDE.md so this is not re-diagnosed next time.

What text extraction had silently dropped - this was not a cosmetic gap:
- p15: the T-shaped quote is attributed to **Prof. Tina Seelig**, Executive Director of the Stanford Technology Ventures Program. The first pass had no attribution at all.
- p22: both Duckworth equations (Effort x Talent = Skill; Skill x Effort = Achievement) and the entire four-panel "How to Grow Your Grit" content - the Bezos quote, the two reflective questions, the 16,000-person purpose survey, the Grit Scale correlation, and the fact that hope means agency rather than optimism. Read by cropping the page into four quadrants at 260 dpi.
- p17-18: the course structure is a **honeycomb of twelve tiles**, not the "jigsaw" the transcript's metaphor implied. Adjacency is meaningful and Technical Know-How is one tile of twelve - the T-shape claim drawn. Promoted to a new concept, L1-C12.
- p19: the full fixed/growth self-talk lists.
- p24: the two lines share an origin and the growth line **branches off** partway along; the course is positioned at the branch point. The first pass had described two separate lines.
- p20 confirmed as a blank video placeholder - nothing lost.

Also added L1-C11 (neuroplasticity) as its own concept; it was buried inside C03 but it is what licenses the hope pillar of C04, so it earns an ID.

Concepts 10 -> 12. Flashcards 52 -> 84. Six figures exported to notes/figures/ and embedded inline.

Per the user's instruction, CLAUDE.md gained two new standing rules: section 3.3a (extract visuals from the slides, prefer them over generated diagrams, zoom into dense slides, never infer a figure from surrounding text) and section 3.3b (format for Obsidian - frontmatter, callouts, collapsible blocks, internal links, tables, LaTeX). All three L1 note files were rewritten to that standard.

Quiz: still none. All 12 concepts remain untested.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. 12 items due 2026-07-28, all L1, all never tested. SE761 L2 has 10 more due the same day - interleave them, do not block by course.
3. Run a Mode B quiz round. The newly recovered material is the most valuable to test because it was never in the notes before: the Duckworth equations, the four pillars with their reflective questions, hope-as-agency, and what the honeycomb encodes.
4. ENGGEN403 L2 and L3 are still completely un-ingested and both have decks + transcripts. L2 is systems thinking and is diagram-heavy - now safe to ingest properly.
5. Still unresolved: the marshmallow/Dunedin attribution, and the exact week for each of the strategic/economic/financial cases on slide 18.
