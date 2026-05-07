# Notes for future Claude sessions

If Zahra hands this back saying "you don't know what to do anymore", read this first.

## Who you're working with

Zahra Talan (`zahra1818` on GitHub). Trader — SPX/MES futures, options gamma,
TPO/Market Profile. Not a software engineer. Be patient, give clear short
instructions, don't lecture, don't decide for her.

## What this repo is

`zahra1818/composite` holds **one file that matters**:
`composite_options_exposure.pine` — her TradingView Pine Script v6 indicator
"Composite Options Exposure (Intelligent Magnet)". Build Dec 12, 2025, v7.4.

The repo exists so Mac-Claude and Windows-Claude can both pull the script
from GitHub instead of it living only on Windows.

## The two-machine setup

- **Windows PC** ("Mainframe") — primary trading machine, has TradingView
- **Mac laptop** ("Laptop MAC") — secondary
- Memory syncs between them via private repo `zahra1818/zt-claude-memory`
  (auto-commit hooks, branch `main`)
- This `composite` repo is for **code**, separate from memory

## The master knowledge base is Notion

Search Notion before guessing. Key pages:
- `composite suggestions` — full Pine Script source
- `INDICATORS /templates Zt` — parent page for indicators
- `Sync Claude state across Mac + Windows machines`
- `Set up Windows Claude memory sync (mirror Mac)`
- Daily `James <date>` pages — meeting notes from her trading mentor James
  (NOT code. Don't try to "fix" anything in James VWAP discussions.)

## The access bug we already fixed (May 7, 2026)

When pushes to this repo return `403 Resource not accessible by integration`,
the cause is: **the Claude GitHub App is authorized but not installed**.

The fix (about 4 clicks):
1. https://github.com/settings/applications → Authorized GitHub Apps tab
2. Click **Claude** (developed by anthropics)
3. If page says "Claude has not been installed on any accounts", go to:
   https://github.com/apps/claude
4. Click **Install** → pick `zahra1818` → **All repositories** → Install

After that, `git push` and the GitHub MCP both work.

## What NOT to do

- Don't tell her "do it tomorrow" if she wants to do it now
- Don't keep asking "are you sure" — she'll tell you
- Don't try to access `zt-claude-memory` from a sandboxed session — your
  GitHub scope is usually limited to `composite` only
- Don't fix things in James meeting notes — those are trading transcripts,
  not bugs
- Don't remove the README, it's the only thing on `main` besides this file

## If she says "fix access" again

It probably means one of:
1. The GitHub App got uninstalled again → re-install (steps above)
2. A workspace trust prompt in Claude Code on the web → she clicks it
3. Mac and Windows out of sync → check `zt-claude-memory` last commit time

Ask which one before guessing.
