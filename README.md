# 1623 NE 73rd Ave house archive

Working historical record for **1623 NE 73rd Ave, Portland, OR 97213** (Lots 27 & 28, Block 33, Jonesmore).

This is not a title report or legal ownership opinion. Every claim in this archive is tied to a source. Oral history counts as a source; it is labeled as oral history until a document corroborates it.

## How to use this archive

1. Read **[house-history.md](house-history.md)** for the sourced narrative.
2. Read **[CONFLICTS.md](CONFLICTS.md)** for what is still open. Recorded calls are in **[decisions.md](decisions.md)**.
3. Use **[timeline.md](timeline.md)** as the dated working record (authoritative order for events).
4. Next records to pull: **[research-queue.md](research-queue.md)** (Fern probate + 1986–1992 deeds for parcel **R193918**).
5. Latest untranscribed image intake: **[2026-08-18 screen-capture intake](sources/ingested/research-notes/2026-08-18-screen-capture-intake.md)**. Its machine-readable checklist is `data/screen-capture-intake-2026-08-18.yaml`.
6. Add new photos, deeds, and notes under `sources/ingested/` and log accepted sources in **[sources.md](sources.md)** and `data/sources.yaml`.

## Folder layout

| Path | What it holds |
| --- | --- |
| `house-history.md` | Sourced narrative history (read this first) |
| `timeline.md` | Chronological working record with certainty and sources |
| `people.md` | People connected to the house |
| `physical.md` | Building, systems, lot, and later work |
| `photos.md` | Photo and map inventory |
| `oral-history.md` | Firsthand and neighbor recollections, each as evidence |
| `sources.md` | Source register (P, O, W, S, M, PL) |
| `CONFLICTS.md` | Open contradictions waiting for your call |
| `decisions.md` | Resolved or working calls, with the date they were made |
| `research-queue.md` | Next records to hunt |
| `photos/` | Named working copies (permits, aerials, genealogy, clippings, plans) |
| `sources/ingested/` | Unaltered originals (Word docs, newspapers, Portland Maps, research notes) |
| `sources/extracted/` | Images and plaintext pulled from the Word files |
| `data/` | Machine-readable YAML mirrors of accepted sources, people, and events, plus intake manifests — keep authoritative mirrors in sync with the markdown |

## Source documents ingested

| ID | File | Created / assembled |
| --- | --- | --- |
| S2022 | `sources/ingested/2022-original-notes/1623 NE 73rd Ave.docx` | Word notes by Rod Young, created 2022-01-19, last saved 2022-04-11 |
| S2026 | `sources/ingested/2026-evidence-report/1623_NE_73rd_Ave_House_History_Evidence_Report_2026-08-16.docx` | Evidence report assembled through 2026-08-16 |
| S2026b | `sources/ingested/research-notes/2026-08-17-follow-up-research.md` | Owner-supplied follow-up, 2026-08-17 |

Also ingested: Portland Maps aerials (1962–2025), 2018 firepit plan, *Oregon Journal* 12 Jan 1951 clipping (W26), and research notes under `sources/ingested/research-notes/`.

## Certainty scale

Borrowed from the 2026 report and used throughout:

| Level | Meaning |
| --- | --- |
| 5/5 Confirmed | Direct primary or authoritative public record |
| 4/5 Very strong | Primary record plus a small identity inference, or strong firsthand oral history |
| 3/5 Probable | Fits the evidence; a linking record is still missing |
| 2/5 Possible | Plausible; large documentary gap |
| 1/5 Unverified lead | Recollection, secondary genealogy, or a lead not yet established |

Oral history can be 4/5 when it is firsthand and specific. It still stays tagged `oral-history` until a document is found.

## Rules for adding evidence

- One claim, one or more source IDs. No unsourced sentences in the timeline.
- If two sources disagree, add a conflict in `CONFLICTS.md`. Do not silently pick a winner.
- Keep original files in `sources/ingested/`. Put working copies and renamed scans in `photos/`.
- New binary captures may remain in an intake manifest until their visible text and source identity are verified; only then promote them into `sources.md` / `data/sources.yaml`.
- When you resolve a conflict, move it to `decisions.md` and update `timeline.md` and `house-history.md`.
- Put new events in **date order** in both `timeline.md` and `data/events.yaml`.
- One person, one section in `people.md` (occupancy and later grantor status belong together).
