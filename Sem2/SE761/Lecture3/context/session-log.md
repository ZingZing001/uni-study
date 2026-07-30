# SOFTENG 761 Lecture 3 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-07-30 - Mode A ingest - device: macbook
Covered: full ingest of Lecture 3 (Mon 27 Jul, the Agile + Scrum lecture). Wrote L3-notes.md (13 concepts, L3-C01 to L3-C13), L3-summary.md, and L3-flashcards.tsv (102 atomic cards, validated exactly one tab per line). Ingested together with Lecture 4 in the same session.

**This lecture closes the gap L2 left open.** The Canvas "Contents of Module 1 and 2" index lists three topics - From Idea to Rationale, Agile, Scrum and Kanban - and L2 delivered only the first. This lecture delivers the other two. So Modules 1 & 2 are now fully covered.

**Canvas source material was deliberately NOT duplicated.** Per the user's instruction, this lecture continues to use `Lecture2/resources/canvas-modules-1-and-2-pages.md`, which is already committed. Lecture3/resources/ therefore holds only the transcript. The cross-reference is recorded in three places so it stays discoverable: the Sources callout at the top of L3-notes.md, `resources_seen.supplementary` in progress.json, and the syllabus map. The Scrum Primer (Canvas Module 3), which that same file records, is named by the lecturer as the team's standing reference and is worth fetching if the browser session is available.

Signal/noise: heavy admin content in the first third - assignment 1 work time, team formation, project bidding, Ed Discussion, lab hours, venue - all quarantined into admin-and-dates.md. Kept as signal the things that look administrative but are actually transferable engineering rules: commits-as-evidence-of-contribution (it is a claim about how invisible work behaves, not a marking mechanic), the code-quality-in-meeting-one instruction, and the escalate-before-week-ten reasoning (remediation takes time, not "be patient").

The 20-question Canvas formative quiz was walked through in class with answers. It is recorded as a **collapsible appendix in the notes, labelled source material** - not as a quiz round. The answers were given, so it is not retrieval practice, and quiz-history.md says so explicitly to stop a future session double-counting it.

Transcript quality is fair, and the failure is unusual: roughly the first 200 lines are near-unusable student crosstalk, while the lecturer's own delivery is largely intact. Confirmed garbles are tabulated in admin-and-dates.md - "scumbags" for Scrumban, "Donne" for Done, "Platonov" for product owner, "the 8 discretion" for Ed Discussion. Two of the twenty quiz questions could not be separated from the crosstalk; eighteen are captured.

Cross-lecture reconciliation done in this pass:
- **L2-C08 (client vs product owner) is now superseded.** L3-C09 gives the full role set and L3-C05 gives the PO-absence protocol. The open item carried in L2's log since 27 Jul - "merge L2-C08 into the fuller Scrum roles when they arrive" - is now resolvable; L2-C08 should be demoted to a pointer on the next pass through that file.
- **L1-C03 (SM is not a PM) and L3-C09 agree** and now cross-link. L3 adds the mechanism: facilitation and impediment removal.
- **L2-C05 -> L3-C07** is the real spine of the course so far: needs become user stories become acceptance criteria become tests.

One thing the lecturer promised and did not deliver: teamwork-risk research from his own last-couple-of-years work, previewed as "next lecture". L4 was the paper-plane simulation instead. Logged as an open question rather than assumed dropped.

Quiz: none. All 13 concepts are notes-written-untested, scheduled for first retrieval 2026-07-31.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **Stop ingesting.** SE761 now has 33 untested concepts (L1 10, L2 10, L3 13) plus L4's 12, and ENGGEN403 has its own backlog. Nothing in SE761 has ever been quizzed. The next session should be Mode B, full stop.
3. When you do quiz L3, prioritise **C02, C03, C09, C12** - they are Assignment 2's content and the assignment is due Friday 7 August. C04 and C08 matter most for the project itself.
4. Predictable misconceptions to watch for: reading "X over Y" as "Y is worthless"; naming "the agile principles" collectively instead of individually; confusing sprint review with sprint retrospective; answering "velocity chart" for the transparent view of product state; treating perfective maintenance as a taste dispute rather than a transparency failure.
5. On the next pass through L2-notes.md, demote L2-C08 to a pointer at L3-C09/L3-C05.
6. Consider fetching the **Scrum Primer** from Canvas Module 3 into Lecture3/resources/ - the lecturer treats it as the team's standing reference and it would let notes cite exact wording for the three pillars.
