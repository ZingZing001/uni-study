# SOFTENG 761 Lecture 1 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-07-27 - Mode A ingest - device: windows-desktop
Covered: full ingest of Lecture 1 (course introduction). 40-page deck with a text layer, plus a ~1,350-line auto-generated transcript. Wrote L1-notes.md (10 concepts), L1-summary.md, L1-flashcards.tsv (63 cards, validated). Three figures exported and embedded.

This lecture is roughly **75% administration** and the signal/noise filter did most of the work. Everything on the teaching team, contact routes, room bookings, prerequisites, deliverable weightings, the week-by-week schedule, GitHub setup and academic-integrity policy went to admin-and-dates.md. What survived: the two assessment axes, the Bloom ladder, the Scrum Master correction, the PO/client fusion, the sprint cycle and the Spike, imposter syndrome, Dunning-Kruger, and the Gen AI pillars.

Three things worth recording:
- **Slide footer numbers run one behind PDF page indices.** Caught it after rendering the wrong pages first. Figures are cited by printed slide number.
- **Transcript quality is poor** - it mangles nearly every proper noun (the lecturer becomes "Reza Shah Hamidi", Paramvir becomes "Farmville" and "premiere", Hoda becomes "hotel", BE(Hons) becomes "Beyonce", Spike becomes "Prince2"). Slides treated as authoritative throughout; the garbles are logged rather than guessed at.
- **A genuine slide/transcript conflict:** slide 17 says the course does NOT count toward professional work hours; the transcript says it can be claimed as internship hours. Flagged in admin-and-dates.md as a question, with the slide trusted.

The most valuable content was in the images. Slide 25 carries the entire five-activity sprint cycle as a diagram - text extraction returned only "7 Sprints / Each sprint is one week". Slide 33 carries the full Dunning-Kruger curve with its five monologue captions; extraction returned only "Mount Stupid" and "Valley of Despair".

Also note the integrative point (L1-C09), which is the reason the two psychology concepts are in the deck at all: imposter syndrome and Dunning-Kruger are opposite states on one axis, and the lecturer's argument is that starting a project *without* imposter syndrome is a warning sign.

Quiz: none. All 10 concepts untested, scheduled 2026-07-28.

**Ingest order problem:** SE761 has been ingested out of order - L2 first, then L1. L1-C04 (Product Owner vs client) and L2-C08 (client vs product owner) cover the same ground from different angles. They should be reconciled rather than left as two half-answers.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. Due 2026-07-28: 10 from SE761 L1, 10 from SE761 L2, 12 from ENGGEN403 L1. That is 32 never-tested concepts across three lectures - too many for one round. Cap at 10 and interleave across all three courses.
3. Reconcile L1-C04 with L2-C08 into a single treatment of client / product owner / user.
4. Expect Agile, Scrum and Kanban next in SE761 - the Canvas contents page lists them and neither lecture has covered them yet.
