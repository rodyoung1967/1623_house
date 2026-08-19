# Source-file layout

This directory preserves evidence and provenance.

- `ingested/` — preserved source documents and captures: Word files, census saves, newspaper screenshots, genealogy captures, plans, and source-provider downloads.
- `extracted/` — text and embedded images extracted from compiled source documents. These are derived from an ingested file and should retain that provenance.

Project-created analysis, transcriptions, search notes, and research methods belong under `research/notes/`, not under `sources/ingested/`.

Named convenience copies used by the narrative are kept under `photos/`. Some are byte-for-byte identical to a file under `sources/ingested/` or `sources/extracted/`; Git stores identical blob content once, so those parallel paths preserve usability/provenance without duplicating the underlying Git object.

Stable source IDs are defined in `../sources.md` and mirrored in `../data/sources.yaml`.
