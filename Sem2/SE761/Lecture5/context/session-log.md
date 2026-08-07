# SE761 Lecture 5 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-08-07 - Mode A ingest - device: macbook
Covered: full ingest of Lecture 5 (reflection models and teamwork risks). Video transcript plus three handout PDFs. Wrote L5-notes.md (11 concepts), L5-summary.md, L5-flashcards.tsv (95 cards, validated). Two figures exported.

Set up the canonical folder structure for L5 and L6, which did not exist - the files were sitting loose at the lecture-folder root.

**The single most useful thing in this lecture is a pointer, not a concept.** The lecturer states outright that **Gibbs' Analysis phase is what Assignment 2 asks for**, and Gibbs' cue question "how do past experiences compare to this?" is the A2 three-mark rubric line almost word for word. That connection turns a generic reflection handout into a report structure. It is written up in L5-C02 and cross-linked from the A2 brief note.

Three other things worth holding.

**The risk/issue distinction (C11)** is the crispest single idea: "as long as you have not started things, they are risks... then there is a potential that they will be converted into real issues." **Risks are mitigated; issues are resolved.** And the failure mode is not mishandling a risk - it is not recognising a situation as a risk at all.

**The risk table is better than the risk list.** The handout's page 2 gives impact, likelihood and priority for all fifteen, and reading it as a table rather than a list produces things the lecture never said aloud: R2 poor communication is the *only* High/High entry, which corroborates the claim that it is the most common cause of risks becoming issues; only three risks (schedules, skills, personality) are Medium priority; and R1 and R3 get different mitigations for a similar-sounding problem - a tool fix versus a Team Charter.

**XP's definition is unusually quotable** and lands in the 1-mark A2 criterion: "whatever good practices are implemented in traditional software development methodologies, we use them, and we use them in an extreme manner." Code review every sprint becomes pair programming - review continuously - "so that means it is a kind of continuous reflection as well." That is a better answer than listing XP practices.

Two counter-intuitive details captured: **volunteering for extra workload is itself a risk** (burnout, and the same single-point-of-failure as dependency on key members), and **decision-making conflicts are a partly positive signal** because they mean everyone is present and contributing.

Source quality is the worst in the course so far - a recorded video with a live room, so student contributions are patchy and several documents are narrated rather than shown. Where the handout PDFs exist they are authoritative, and the transcript artefacts are catalogued in admin-and-dates.md ("models of infection" for reflection is the memorable one).

Quiz: none. All 11 concepts untested, scheduled 2026-08-08.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. Get the answers to **risk quiz Q14-Q19** - not covered on the recording. Q15 is the interesting one ("All of the above" is an option).
3. When quizzing L5: lead with **C02** (Gibbs' six stages and the four Analysis cue questions), **C11** (risks mitigated vs issues resolved), **C10** (which risk is High/High, and the mitigations for R3, R6, R12), **C07** (retrospective vs review).
4. ⚠ The two risk PDFs live in `Lecture6/resources/` but are L5 content. Moving them breaks references in `L5-notes.md` and `Lecture5/context/progress.json`.
5. **The retrieval debt still applies**: SE761 now has L1-L6 ingested and zero quiz attempts across the whole course.
