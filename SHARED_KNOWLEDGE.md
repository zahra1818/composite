# Shared Knowledge — Mac ↔ Windows Claude

Single source of truth for everything both sessions need to know.
Append-only by default. Refine in place; do not delete history.

---

## Project

- TradingView indicator: **Composite Options Exposure (Intelligent Magnet)**.
- Pine Script source of truth lives in this repo.
- Source previously lived only on the Windows machine. Goal: parity
  between Mac and Windows Claude sessions.

## Volsignals

_(empty — fill in as we learn)_

## Indicators / Setups

_(empty)_

## Decisions

- 2026-05-08 — Established this repo as the daily sync bridge between
  Mac and Windows Claude sessions. Protocol in `CLAUDE.md`.
- 2026-05-08 — Windows Claude built an OneDrive-based sync between
  Windows Desktop Claude and Mac Desktop Claude. **Limitation:**
  Browser Claude (Claude Code on the web) is sandboxed Linux and
  cannot read OneDrive, so it is excluded from the OneDrive bridge.
  See `MESSAGE_TO_WINDOWS.md` for the proposed fix (Option A
  dual-write to git, or Option B git as single source of truth).

## Open Questions

- [for windows] Push the current Pine Script source from the Windows
  machine into this repo so the Mac session can see it.
- [for windows] Pick Option A or B from `MESSAGE_TO_WINDOWS.md` and
  push the current memory snapshot (Volsignals, Dan's Discord,
  morning prep routines) into `composite` under `memory/`.

## Disagreements

_(empty)_
