---
course: SE761
type: design-note
title: Backlog audit against the architecture decisions
date: 2026-08-19
status: revised after reading the actual board
tags: [se761, project, backlog, jira, audit]
---

# Backlog audit — SCRUM board, Agile Avengers

> [!important] This file was rewritten
> The first version assumed the board contained only scaffolding, based on the ten ticket numbers audible in the 18 Aug standup transcript. **That assumption was wrong.** The board is 96 issues across 10 epics and already covers the product end to end. Most of what the earlier version recommended adding already exists.

**Audited directly:** all 10 epics · SCRUM-24 Care Plan stories (5 of 8) · SCRUM-28 Adherence stories (5 of 7).
**Not read individually:** stories under SCRUM-21, 22, 23, 25, 26, 27, 29.

---

## Epic structure

| Epic | Scope |
|---|---|
| SCRUM-6 | Sprint 1 — Spike and Release Planning |
| SCRUM-21 | Platform Foundation |
| SCRUM-22 | Identity and Access Control |
| SCRUM-23 | Patient and Caregiver Management |
| SCRUM-24 | Care Plan — Prescriptions, Medication and Exercise |
| SCRUM-25 | Clinical Web Portal |
| SCRUM-26 | Virtual Care Agent (phone client) |
| SCRUM-27 | CARE Server Integration |
| SCRUM-28 | Adherence History and Oversight |
| SCRUM-29 | Deployment and Operability |

This is already the structure the earlier draft recommended restructuring *towards*. No change needed.

---

## Recommendations that were already implemented

| Earlier recommendation | Where it already lives |
|---|---|
| Add missed-dose handling | **SCRUM-90** (caregiver sees missed doses) and **SCRUM-91** (notify caregiver) |
| Make confirmation events append-only | **SCRUM-53**: "past events are unchanged". **SCRUM-55**: "Past events and their history are never rewritten" |
| Question self-registration for clinical roles | **SCRUM-22** epic already carries it as an open PO question, in the same terms |
| Generalise exercise alongside medication | **SCRUM-54**, with PO confirmation recorded |
| Build CARE behind a mock | **SCRUM-27**: "Build against a mock from day one. No demo may ever depend on CARE being up" |
| Deploy early and keep it deployed | **SCRUM-29**: "If the final demo runs only on localhost, we have rebuilt their problem" |

---

## What still genuinely needs changing

### 1. SCRUM-52 conflicts with the shared-catalogue model — the one real defect found

> **SCRUM-52 acceptance criteria:** "Each medication carries name, dose, and free-text instructions"

As written, medication name is typed per prescription. That means the same drug exists as many independent strings across patients.

**Consequences:** no way to query across patients by drug; typos become distinct medications; and **federation with the CARE hub becomes a string-reconciliation problem instead of an ID mapping.** Given SCRUM-27 now says the hub reads data *from* us, this is the expensive one to get wrong.

**Change to:** a `Medication` catalogue entity that prescriptions reference by ID. Dose and instructions stay on the prescription line — they are per-patient. Name, form and strength move to the catalogue.

**Add a story:** manage the medication catalogue (create, search, supersede). Same for exercise.

### 2. Bidirectional integration is not reflected in the architecture

SCRUM-27 records something not previously captured: **the CARE hub retrieves data from us**, so we must expose an inbound authenticated API for a consumer we cannot see yet. See the updated §6a of [[architecture-review]].

**Add a story** under SCRUM-27: expose a read API for the hub, with authentication, a versioned contract, and its own tests. It is not free and it is not the same work as the outbound adapter.

### 3. External identity mapping is missing

Nothing yet covers mapping our identifiers to the hub's. **Add:** an `ExternalReference (localId, externalSystem, externalId)` concept and a story to maintain it. Cheap now, expensive after data exists.

### 4. Activities are absent from the backlog

Cole's demo showed brain games, karakia, entertainment and appointments running on the robot today. None appear in the epic structure.

**This may be deliberate scoping, and if so it is a good decision** — but it must be *visible* as a decision. The use case diagram should show the full domain with our scope marked, or a marker reads the omission as not having understood the product.

### 5. Define "postponed"

SCRUM-89 lists four outcomes: taken, skipped, postponed, missed. Postponed is the only one whose semantics are not obvious — does it re-arm the reminder, and does it become missed later? Pin it down before SCRUM-89 is built, since it changes the state machine.

---

## Blocked items needing the PO — carry to the next contact

1. **SCRUM-91** — is a missed dose record-only, or does someone get alerted? Already flagged BLOCKED on the ticket.
2. **SCRUM-29** — who hosts and who pays. Already flagged BLOCKED.
3. **SCRUM-22** — who approves a healthcare-professional account.
4. **SCRUM-27 → ask Jay** — does CARE expect a fixed schema, or adapt to ours? Guessing wrong is rework in Sprint 5–6.

---

## Verdict

The backlog is DEEP: detailed, prioritised, epic-structured, with acceptance criteria in given/when/then form and blockers surfaced on the tickets themselves. It is in better shape than the Project Proposal requires.

The remaining work is **five targeted changes**, not a restructure — and item 1 is the only one that is a defect rather than an addition.
