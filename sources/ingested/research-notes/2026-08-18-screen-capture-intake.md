# 2026-08-18 screen-capture intake

Source commit: `04126ebeac2f103153cbb0e332e283b907d20f6b` (`new photos`).

This note records the latest screen captures after archival organization. The binary files were moved from repository root into canonical `sources/ingested/` locations and, where useful for daily work, mirrored under `photos/genealogy/` using the same Git blob. No image was recompressed and no source content was discarded.

## Evidence rule for this intake

The GitHub connector used for this processing pass can preserve and identify the binary files but cannot expose their pixels for reliable visual transcription. Therefore **no historical claim is created or conflict closed from a filename alone**. Filename wording is retained as user-supplied provenance/intake metadata only. Each capture below remains `needs-visual-transcription` until its visible text, date, page/masthead, names, addresses, and context are checked.

## Census / NARA material

### 1940 Census 1623 capture
- Original upload: `1940 Census 1623.png`
- Git blob: `102b6feeff986d69450f1826a3c78cca0f2817eb`
- Canonical original: `sources/ingested/census/1940-census-1623-page-capture.png`
- Working copy: `photos/genealogy/1940-census-1623-page-capture.png`
- Candidate relationship: potential upgrade to `P7`, which is currently only an Ancestry summary screenshot.
- Must verify visually: enumeration district, sheet/page, line numbers, street and house number, household names, owned/rented field, home value/rent, and all other fields actually visible.
- Do not upgrade P7 to original-sheet status until that check is complete.

### NARA 1940 enumeration-district description save
- Original upload: `1940 Census Enumeration District Descriptions - Oregon - Multnomah County - ED 37-228, ED 37-229, ED 37-230.htm`
- Git blob: `ab6d3245e367610c9e6feec1a15d30f687376f84`
- Canonical path: `sources/ingested/census/1940-nara-ed-descriptions-37-228-37-230.htm`
- Saved from National Archives Catalog ID `5878834`.
- The saved page explicitly describes `OR ED 37-228`, `OR ED 37-229`, and `OR ED 37-230` as Portland City enumeration districts in election precincts 164/165.
- Important limitation: this finding-aid page by itself does **not** establish which of those EDs contains 1623 NE 73rd Ave. That link must come from the census page/address or an ED map/street-boundary check.

## Newspaper and genealogy captures

| Intake item | Canonical working copy | Possible existing relationship | Required follow-up |
| --- | --- | --- | --- |
| `945-11-01-james-b-deveny-funeral-notice  part 2.png` | `photos/genealogy/1945-11-01-james-b-deveny-funeral-notice-part-2.png` | Compare with `W33` | Determine whether this is continuation/alternate crop of W33; transcribe survivors, residence, publication/date/page. |
| `Denise Genevieve Dowty Birth Notice Oregonian.png` | `photos/genealogy/1967-denise-genevieve-dowty-birth-notice-oregonian.png` | Compare with `W29` | W29 is currently an *Oregon Journal* 7 Jun 1967 notice. Determine whether this is a separate *Oregonian* notice or only an alternate/mislabeled capture before assigning a new source ID. |
| `Deveney Oregon Journal September 21, 1920.png` | `photos/genealogy/1920-09-21-oregon-journal-deveney.png` | New candidate source | Transcribe the DeVeny name(s), address(es), event, and page. Assess relevance to `C03` / early DeVeny family identification only after text is known. |
| `Fern Funeral Notice Oregonian.png` | `photos/genealogy/fern-deveny-funeral-notice-oregonian.png` | New high-priority candidate | Transcribe exact date/page, residence, place-of-death wording if any, survivors and service details. Highest priority for `C10` (Fern at 1623 / death in house). Do not treat a funeral notice as proof of place of death unless it explicitly says so. |
| `Irene Funeral Notice.png` | `photos/genealogy/irene-f-taylor-funeral-notice.png` | New candidate source | Identify publication/date and confirm whether this is Edgar and Fern's daughter Irene F. Taylor; extract residence, spouse/children, dates, and family links. |
| `James B Deveny Funeral Notice Oregonian.png` | `photos/genealogy/1945-james-b-deveny-funeral-notice-oregonian.png` | Compare with `W33` | Determine whether this is W33 from another crop/publication or a distinct notice. The filename's `Oregonian` label is not treated as verified masthead evidence until checked. |
| `Nola Deveny Marriage Licence to Lloyd Oregonian.png` | `photos/genealogy/1952-nola-deveny-lloyd-dowty-marriage-license-oregonian.png` | New candidate source | Determine whether it records a license application/issuance or completed marriage; transcribe date and parties. Could resolve the exact 1952 Dowty marriage date, but a license date must not be substituted for a wedding date. |
| `Nola Deveny Wedding to Lloyd Oregonian.png` | `photos/genealogy/1952-nola-deveny-lloyd-dowty-wedding-oregonian.png` | Compare with `W30` | Verify masthead/publication date and wedding date. W30 currently has a working 20 Sep 1952 inference from a supposed 26 Sep clipping; this capture may confirm or correct that. |
| `Sophia Devny.png` | `photos/genealogy/sophia-deveny-capture.png` | New candidate / document type unknown | Identify what record/site is shown and transcribe name spelling, dates, relationships and maiden name. Relevant to `C16` only if the source actually supplies the maiden name. |
| `Sophie Devny Obituary Oregonian.png` | `photos/genealogy/sophia-deveny-obituary-oregonian.png` | New candidate source | Transcribe exact name spelling, publication/date/page, residence, spouse/children, maiden-name wording if present. Could bear on `C03` and `C16`; do not infer parcel ownership from family relationship alone. |

Canonical originals for the newspaper captures are in `sources/ingested/newspapers/`; the Sophia non-obituary capture is in `sources/ingested/genealogy/`.

## What can be accepted now

1. The repository now contains a higher-resolution / page-style 1940 census capture candidate in addition to the older P7 summary.
2. The NARA saved page is a valid finding aid for ED 37-228 through 37-230, but it does not yet link 1623 to a specific ED.
3. The new captures create concrete follow-up evidence paths for Fern, Irene, James/Sophia, the 1920 DeVeny family, Nola/Lloyd's 1952 marriage, and Denise's 1967 notice.
4. No existing historical conclusion is overturned by this intake pass, because the image text has not yet been visually verified.

## Close-out checklist

After visual transcription, for each item:
1. decide whether it is a new source or an alternate capture of an existing `W#`/`P#`;
2. add or update the stable source ID in `sources.md` and `data/sources.yaml`;
3. add a short plaintext transcription/summary under `sources/ingested/research-notes/`;
4. update `timeline.md`, `people.md`, `house-history.md`, `CONFLICTS.md` / `decisions.md`, and YAML mirrors only for claims actually supported;
5. remove the corresponding `needs-visual-transcription` item from this intake note once integrated.
