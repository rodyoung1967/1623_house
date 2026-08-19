# Repository structure and data-consistency audit — 2026-08-19

Scope: entire `1623_house` repository after the 2026-08-18 evidence integration.

## Findings and actions

### Structure

1. **Project-created research notes were mixed into `sources/ingested/`.** They were moved to `research/notes/`; preserved source evidence remains under `sources/ingested/`.
2. **The extracted text for S2026c was stored beside the ingested DOCX.** It was moved to `sources/extracted/2026-08-17-house-history/extracted-text.txt`, matching the archive's other derived extraction output.
3. `photos/` contains named working copies that sometimes duplicate a byte-identical file under `sources/ingested/` or `sources/extracted/`. This is intentional and retained: the paths serve different purposes, and identical Git blobs are stored once in the object database.
4. `sources/ingested/census/1940-nara-ed-descriptions-37-228-37-230.htm` is not the ED evidence for this house. It is retained as an intake/finding-aid artifact and explicitly labeled as such; P7 independently establishes ED 37-308.
5. Directory conventions are now documented in `research/README.md`, `sources/README.md`, and `data/README.md`.

### Data consistency

1. The 2026-08-17 follow-up note contained the pre-W39 oral-history statement that Fern died in the house. The note is preserved as a research snapshot but now clearly marks that detail **superseded** by W39, which places her death at Friendship Care Center.
2. The same note described Edgar's 1969 notice as proving a “death place” at 1623. The actual notices establish **residence**, not place of death; the research note now states the narrower supported claim.
3. The 1945–1957 clipping note retained the old inferred September 1952 Nola/Lloyd wedding date and an uncertain 19 Aug 1871 reading for James Benjamin DeVeny. W37 directly establishes **8 Nov 1952**, and W35 gives **14 Aug 1871**. The old readings remain visible as superseded research history rather than being silently deleted.
4. The 2026-08-17 research-guide note said the 1950 census was not yet retrieved; it now records that P8 was retrieved on 2026-08-18.
5. Machine YAML used both `conflict:` and `conflicts:` at the top level. Top-level unresolved issue references were normalized to `conflicts: [C##, ...]` while preserving the underlying conflict information.
6. `data/events.yaml` cited W27 on the 1967 Denise birth event even though W27 is Edgar's 1969 death notice. The unrelated citation was removed from that event; W29/W38 remain the proper sources.
7. Paths in `README.md`, `sources.md`, `photos.md`, `research-queue.md`, `data/sources.yaml`, and the screenshot intake manifest were synchronized with the new research/extraction layout.

## Reviewed with no factual changes required

- `house-history.md`
- `timeline.md`
- `people.md`
- `physical.md`
- `oral-history.md`
- `decisions.md`
- `CONFLICTS.md`
- `needed-records.md`

These current narrative files are consistent on the major resolved points: P7's 1940 census reading, Nola's 4 Nov 1952 address, the 8 Nov 1952 Dowty wedding, Fern's 1986 place of death, Nola's Milwaukie evidence, Goodwin spelling, and the Fern-not-Nola elderly-resident conclusion.

## Content-removal review

**No unique evidence, stable source ID, or factual content was removed in this audit.** Files removed from old paths were path moves after their content was preserved under the new structure. Temporary maintenance placeholders contained no evidence and were removed.

Apparent duplicates such as working copies in `photos/`, W4/W14's related Find a Grave material, and the non-house-ED NARA finding-aid capture were deliberately retained rather than deleted.

If later cleanup proposes deleting any retained evidence artifact, stable source ID, or unique research content, it should be presented for owner approval before removal.
