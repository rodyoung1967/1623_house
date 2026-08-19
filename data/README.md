# Machine-readable mirrors

These YAML files mirror the accepted human-readable archive.

- `sources.yaml` mirrors `../sources.md`.
- `people.yaml` mirrors `../people.md`.
- `events.yaml` mirrors `../timeline.md`.
- intake manifests record the processing state of new evidence batches.

## Conventions

- Source IDs (`P#`, `W#`, `O#`, `S#`, `M#`, `PL#`) are stable.
- `sources` is always a list of source IDs.
- Top-level unresolved issues use `conflicts: [C##, ...]`, even when there is only one.
- A descriptive `status` may distinguish documented facts, context, oral evidence, disputed dates, and high-confidence inferences.
- Census/directory occupancy or reported tenure must not be promoted to legal title without a recorded instrument.
- When a human narrative changes, update its YAML mirror in the same maintenance pass.
