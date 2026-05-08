# Sync Protocol — Mac ↔ Windows Claude

This repo is the shared brain between the Mac and Windows Claude
sessions. Both sides MUST stay on the same level of information.

## Every session, do this:

1. **Pull first.** `git pull origin main` (or the active branch).
2. **Read `SHARED_KNOWLEDGE.md`** before doing anything else. That is
   the canonical state of what both sides know.
3. **Read today's entries in `log/`** (both `*-mac.md` and
   `*-windows.md`) to catch up on what the other side did.

## Every time you learn something new, do this:

1. **Append to `SHARED_KNOWLEDGE.md`** under the right section
   (volsignals, indicators, setups, decisions, open questions, etc.).
2. **Append to today's log file** for your side
   (`log/YYYY-MM-DD-mac.md` or `log/YYYY-MM-DD-windows.md`) — short
   bullet of what you did or learned.
3. **Commit and push** immediately. Do not batch. The other side has
   to be able to pull at any time and be current.

## End of session:

- Make sure everything is committed and pushed.
- If there are open questions for the other side, put them under
  `## Open Questions` in `SHARED_KNOWLEDGE.md` and tag with `[for mac]`
  or `[for windows]`.

## Rules

- Never delete history from `SHARED_KNOWLEDGE.md`. Only append or
  refine in place.
- If the two sides disagree, write both views down under
  `## Disagreements` and let the user decide.
- Pine Script source of truth lives in this repo. Do not keep edits
  only on the local machine.
