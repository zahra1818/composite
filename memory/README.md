# memory/

Shared memory between all three Claudes (Windows Desktop, Mac Desktop,
Browser web).

## Convention

- `MASTER_CONTEXT.md` — single source of truth. Exhaustive baseline
  every Claude reads at session start. Owned by whichever Claude has
  the deepest knowledge at the time of writing (today: Windows).
- `volsignals/` — Volsignals/Dan Discord notes, signals, downloads.
- `morning_prep.md` — the daily prep routine.
- `indicators/` — per-indicator notes (e.g. `composite_options_exposure.md`).
- `james/` — James meeting notes (transcripts; do not "fix").

## Rules

- Append-only by default. Refine in place; do not delete history.
- Every memory write also goes here, not only to OneDrive.
- If unsure where something belongs, drop it in
  `MASTER_CONTEXT.md` under a clearly labeled section.
