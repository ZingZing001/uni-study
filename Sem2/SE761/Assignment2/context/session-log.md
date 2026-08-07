# SE761 Assignment 2 - Session log

APPEND-ONLY. New entries at the bottom. Never edit or reflow earlier entries.

---

### 2026-08-07 14:56 - brief analysis - device: macbook
Set up the assignment folder structure (`resources/`, `notes/`, `context/`) mirroring the lecture layout, and fixed the folder-name typo `Assginment2` -> `Assignment2`. Moved `A2.pdf` into `resources/`. Wrote `notes/A2-brief.md`.

**No drafting done - this is a reflective assignment and the content has to be yours.** What the note contains is a decode of the brief, not an answer to it.

Three things the brief makes clear that are easy to miss on a first read:

1. **The mark split is lopsided and it is not where most people put their words.** Three of the eight content marks sit on "reflection on previous development experiences and their outcomes; compare them meaningfully with how the outcome might have changed if an Agile approach was followed". That is the largest single block, it is the only part nobody else could write, and the counterfactual - not the anecdote - is the assessed half of it.

2. **The brief threatens a redo.** "If the report reads as a series of 'pros and cons', speaking in general terms, etc., it will come across as being written by ChatGPT. That's not a reflection, and you might be asked to redo the assignment to be more reflective." This is the only place in either A1 or A2 with that language.

3. **A2 inverts A1 on three axes at once.** Gen AI: encouraged and worth 2 marks in A1, discouraged for content in A2. Personal language: banned in A1, permitted in A2. Format: bullet points in A1, full paragraphs in A2. Carrying A1 habits over is a live risk.

The most useful single link is from L5: the lecturer said outright that **Gibbs' Analysis phase is what A2 is asking**, and Gibbs' cue question "How do past experiences compare to this?" is the 3-mark rubric line almost verbatim. That gives a spine for the report without needing to pick a model formally - though the lecturer said that if you do follow one, name it in the submission.

Flagged but not resolved: the L4 open question about whether "one other practice" must be Kanban or XP. The PDF says "or other principles", so a named and justified alternative should be safe.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **Due 9pm tonight, 7 Aug.** If not yet submitted, the checklist at the bottom of `notes/A2-brief.md` is the fastest path to a pre-submission pass.
3. After submitting: set `status` to `submitted` in `progress.json` and append the outcome here.
4. When marks arrive, record the actual feedback. A3 is also 800-900 words and also reflective, so A2's feedback is directly transferable - and L6 shows the lecturer volunteering A1 marking patterns to the class, so the same is likely for A2.

### 2026-08-07 (later) - material mapping - device: macbook
Supplied `runjiacv2026.json` (CV export) and the personal site. The /ask-me page is a client-side RAG chatbot so it returns nothing to a fetcher; pulled the underlying content instead from `ZingZing001/PersonalWebsite-V2` (`src/data/blogPosts.js`), which is where the chatbot's knowledge base is built from anyway. Wrote `notes/A2-material-map.md`.

**Still no prose drafted.** The brief forbids it and the 3-mark block depends on things only the author knows. What the note does is sort existing history against the rubric and pose the questions that only he can answer.

The strongest thing that came out of this is structural rather than anecdotal: **the brief's own framing of the constraint - "a university course, which will have obvious differences to a real-world full-time industry job where you are only focusing on one job at a time" - describes his actual situation almost literally.** He is concurrently a part-time Graduate SWE at EROAD (Tax team), Product Owner at AUSS, on a 4-person capstone team, a GTA, and now in an 8-person SE761 team on one-week sprints. Most of the cohort will write about conflicting schedules abstractly; he can write about it as a fact about his calendar, and about what it does to specific Scrum events.

Three reflection candidates identified, ranked by how much only he could write them:

1. **He has been the Product Owner.** At AUSS he prioritises a Jira backlog for student volunteers and reports to a non-technical exec committee. L1-C04 and L3-C05 are both about what to do when the PO is unavailable - and he has *been* the unavailable PO. In SE761 he flips to the other side. That is an insight unavailable from the Scrum Guide.
2. **EzShift didn't finish.** The CV says "delivered using Agile methodology" and then, a year on, "next steps: finalising the backend framework". The rubric asks for previous experiences *and their outcomes*; an outcome that didn't land is worth more than one that did, if diagnosed rather than apologised for. Likely the single best counterfactual he has.
3. **The EROAD Tax team contradicts an Agile value in a real way.** His own blog: the bar moved from "does the demo work?" to "will this be correct, reliable and maintainable for years?" - which sits awkwardly against delivering working software frequently. He has lived both poles inside one year, and is about to be pushed back to the prototype end by one-week sprints.

Flagged four author-specific traps. The important one: **his CV is unusually strong for a student, and that is a hazard here.** Listing five workplaces would burn 300 words and score in the wrong place; two experiences deep beats five listed. Also flagged that his blog voice is naturally promotional and full of gratitude, which is right for a blog and wrong for a rubric that penalises description over examination.

**HANDOFF - start here next time:**
1. `git pull --rebase --autostash`
2. **Due 9pm tonight.** If the draft exists, review it against the rubric line by line - description-vs-reflection, word count, and whether the past-experience block is the longest section.
3. After submitting: set `status` to `submitted` in `progress.json` and record the outcome.
4. The material map is reusable for **A3**, which is also 800-900 words and also reflective - though A3 is anchored to the allocated project and a research paper rather than to personal history.
