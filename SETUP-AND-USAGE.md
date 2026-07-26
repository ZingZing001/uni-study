# Setup and usage

## What this repo is

A study workspace driven by an AI study partner. The agent's standing brief is [CLAUDE.md](CLAUDE.md) — it defines the folder layout, how lectures get ingested, how quizzing works, and the git protocol. Read that file if you want to know *why* something is structured the way it is; this file is just the mechanics.

## One-time setup on a new device

```bash
git clone https://github.com/ZingZing001/uni-study.git
cd uni-study
```

Tools the agent uses when ingesting slide decks (Poppler utilities):

- Windows: `winget install oschwartz10612.Poppler` (or install Poppler and put its `bin/` on PATH)
- macOS: `brew install poppler`
- Linux: `sudo apt install poppler-utils`

Verify with:

```bash
pdfinfo -v
```

Without these, PDF slide decks can't be read properly.

## Day-to-day loop

1. **Drop files.** Put the slide deck and transcript into
   `Sem2/<COURSE>/Lecture<N>/resources/`.
   Slides as `*.pdf`, transcript as `*.txt` / `*.vtt` / `*.srt` / `*.docx`.
   Never put lecture video or audio in here — it won't be committed (see `.gitignore`).
2. **Start a session.** Open the agent in the repo root. It reads `CLAUDE.md`, pulls, and opens with a one-line status: what's due for review, what's weak, what it suggests.
3. **Say what you want.** The three modes:
   - `Start SE731 Lecture 4` → ingest new material (Mode A)
   - `Quiz me` → retrieval practice on what's already noted (Mode B)
   - `I don't get <X>` → drop everything and re-teach (Mode C)
   - Also useful: `I have 20 minutes` — the agent plans and pushes inside that budget.
4. **End the session.** The agent commits and pushes. If it doesn't confirm the push succeeded, the session is lost — chase it.

## Which files are yours vs the agent's

| Path | Who writes it |
|---|---|
| `resources/` | **You only.** The agent treats it as read-only input. |
| `notes/` | Agent. Yours to read; edit freely if it got something wrong. |
| `context/progress.json` | Agent. Tracks concepts, confidence, review dates. |
| `context/session-log.md` | Agent, append-only. Each entry ends with a handoff block. |
| `context/quiz-history.md` | Agent, append-only. |
| `context/admin-and-dates.md` | Agent. All the deadline/logistics noise, quarantined out of the notes. |
| `course-context/` | Agent. Cross-lecture review queue, weak spots, syllabus map. |

## Adding a new lecture or course

Just ask — "set up Lecture 5" or "add SE754". The agent creates the canonical tree from `CLAUDE.md` §1. Don't hand-roll the folders; the layout is load-bearing.

## Multi-device

Committed state is the only state. The agent pulls with `--rebase --autostash` at session start and pushes at session end. Append-only logs and per-concept JSON merging make conflicts cheap — the agent resolves them itself per `CLAUDE.md` §7 and tells you what it did.

## Flashcards

`notes/L<N>-flashcards.tsv` is tab-separated `question<TAB>answer`, no header. In Anki: **File → Import**, field separator **Tab**, map field 1 → Front, field 2 → Back.
