# 1623 NE 73rd Ave house archive

Working historical record for **1623 NE 73rd Ave, Portland, OR 97213** (Lots 27 & 28, Block 33, Jonesmore).

This is not a title report or legal ownership opinion. Every claim in this archive is tied to a source. Oral history counts as evidence; it remains labeled as oral history and is reconciled when documentary evidence confirms or contradicts a detail.

## How to use this archive

1. Read **[house-history.md](house-history.md)** for the sourced narrative.
2. Read **[CONFLICTS.md](CONFLICTS.md)** for what is still open. Recorded calls are in **[decisions.md](decisions.md)**.
3. Use **[timeline.md](timeline.md)** as the dated working record.
4. Use **[needed-records.md](needed-records.md)** as the master checklist of everything still worth collecting.
5. Use **[research-queue.md](research-queue.md)** for exact offices, contacts, and search instructions for the highest-value records.
6. The latest screenshot batch is documented in **[2026-08-18 screenshot transcriptions](sources/ingested/research-notes/2026-08-18-screenshot-transcriptions.md)**. Its original intake/status log is **[here](sources/ingested/research-notes/2026-08-18-screen-capture-intake.md)** with machine mirror `data/screen-capture-intake-2026-08-18.yaml`.
7. Add new photos, deeds, and notes under `sources/ingested/` and log accepted sources in **[sources.md](sources.md)** and `data/sources.yaml`.

## Current high-value conclusions

- The original 1940 census page is now in the archive as **P7**: ED **37-308**, sheet **1A**, lines 16–19. Edgar, Fern, Irene, and Nola are at 1623; the household reported the home **owned**, value **$1,500**. Census tenure is not treated as a deed (C05).
- **Nola D. DeVeny is directly documented at 1623 N.E. 73d on 4 Nov 1952** (W36), four days before marrying Lloyd Wallace Dowty on **8 Nov 1952** (W37).
- The elderly woman remembered by the neighbor as living alone at the house was **very likely Fern A. DeVeny, not Nola** (C19).
- Fern's 1986 obituary (W39) corrects one detail of that oral history: she **died at Friendship Care Center**, not at 1623. Her last verified date living at the house remains a major research target.
- Nola is documented **of Milwaukie in 1967** (W29) and again in **1987** (W40).
- Sophia's family surname is **Goodwin**, supported by the 1920 James Goodwin notice (W34; C16 resolved).

## Folder layout

| Path | What it holds |
| --- | --- |
| `house-history.md` | Sourced narrative history (read this first) |
| `timeline.md` | Chronological working record with certainty and sources |
| `people.md` | People connected to the house |
| `physical.md` | Building, systems, lot, and later work |
| `photos.md` | Photo and map inventory |
| `oral-history.md` | Firsthand and neighbor recollections, reconciled against documents |
| `sources.md` | Source register (P, O, W, S, M, PL) |
| `CONFLICTS.md` | Open contradictions / unresolved readings |
| `decisions.md` | Resolved or working calls, with dates and evidence |
| `needed-records.md` | Master collection checklist |
| `research-queue.md` | Offices, contacts, searches, and next-record strategy |
| `photos/` | Named working copies (permits, aerials, genealogy, clippings, plans) |
| `sources/ingested/` | Preserved originals and research notes |
| `sources/extracted/` | Images/plaintext extracted from compiled documents |
| `data/` | Machine-readable YAML mirrors of accepted sources, people, events, and intake state |

## Source documents ingested

| ID / group | File | Created / assembled |
| --- | --- | --- |
| S2022 | `sources/ingested/2022-original-notes/1623 NE 73rd Ave.docx` | Word notes by Rod Young, created 2022-01-19, last saved 2022-04-11 |
| S2026 | `sources/ingested/2026-evidence-report/1623_NE_73rd_Ave_House_History_Evidence_Report_2026-08-16.docx` | Evidence report assembled through 2026-08-16 |
| S2026b | `sources/ingested/research-notes/2026-08-17-follow-up-research.md` | Follow-up research, 2026-08-17 |
| S2026c | `sources/ingested/2026-08-17-house-history/1623_NE_73rd_Ave_House_History_2026-08-17.docx` | Compiled working history; some dates later corrected by direct clippings |
| 2026-08-18 review | `sources/ingested/research-notes/2026-08-18-screenshot-transcriptions.md` | Direct visual transcription of P7 and W34–W40 |

Also ingested: Portland Maps aerials (1962–2025), the 2018 firepit plan, historic plumbing/sewer records, census saves, newspaper clippings, and research notes.

## Certainty scale

| Level | Meaning |
| --- | --- |
| 5/5 Confirmed | Direct primary or authoritative public record |
| 4/5 Very strong | Primary record plus a small identity inference, or strong firsthand oral history |
| 3/5 Probable | Fits the evidence; a linking record is still missing |
| 2/5 Possible | Plausible; large documentary gap |
| 1/5 Unverified lead | Recollection, secondary genealogy, or an unestablished lead |

Oral history can be 4/5 when firsthand and specific. A contradicted detail is corrected without discarding unrelated portions of the same recollection.

## Rules for adding evidence

- One claim, one or more source IDs. No unsourced factual assertions in the timeline.
- If two credible sources disagree, add a conflict in `CONFLICTS.md`; do not silently pick a winner.
- Keep original files in `sources/ingested/`. Put working copies and renamed scans in `photos/`.
- New binary captures may remain in an intake manifest until visible text/source identity are checked; then promote them to stable IDs.
- When resolving a conflict, update `decisions.md`, `CONFLICTS.md`, `timeline.md`, `house-history.md`, and the relevant YAML mirrors.
- Put new events in date order in both `timeline.md` and `data/events.yaml`.
- Keep `people.md` and `data/people.yaml` aligned.
- Keep `sources.md` and `data/sources.yaml` aligned.
- Add every meaningful unresolved collection target to `needed-records.md`; put operational details in `research-queue.md`.
