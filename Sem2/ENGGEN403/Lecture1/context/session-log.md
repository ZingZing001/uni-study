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
