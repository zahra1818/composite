# Message to Windows Claude — please do this when you read this

Hey Windows. Zahra is exhausted. Don't ask her clarifying questions.
Just do the work below.

## Why

OneDrive ClaudeSync covers Windows Desktop Claude ↔ Mac Desktop
Claude. It does **not** reach Browser Claude (Claude Code on the web)
because Browser Claude runs in a sandboxed Linux VM with no Mac
filesystem and no OneDrive client. The only channel Browser Claude
can reach is this git repo (`zahra1818/composite`).

Result today: Mac Desktop Claude is freshly synced via OneDrive but
its conversational baseline is still empty. Browser Claude has
nothing. Windows is the only one with deep memory.

## What to do — exactly this, no questions

1. **Read your saved memory** (everything under `~/.claude/projects/`
   and any cross-project memory). Pull from saved memories, not just
   the current chat context.
2. **Compose `memory/MASTER_CONTEXT.md`** in this repo. Be exhaustive.
   Cover at minimum:
   - **Who Zahra is** — trader, SPX/MES futures, options gamma, TPO/Market
     Profile. James is her trading mentor (meeting notes are not bugs).
   - **Volsignals + Dan's Discord** — what the service is, who Dan is,
     what kind of signals/posts she pulls, what she does with them,
     how she's downloading the messages today.
   - **Morning prep routine** — exact steps, in order, with timing.
   - **Composite Options Exposure (Intelligent Magnet)** — what the
     indicator does, current build (v6, v7.4, Dec 12 2025), where the
     source of truth lives, known issues, recent changes.
   - **Other indicators / setups** she relies on.
   - **Open decisions / open questions** that affect either side.
   - **Hard-won lessons** — anything you'd be sad to lose if memory
     wiped tomorrow.
3. **Save the same file** to `~/Library/CloudStorage/.../ClaudeSync/memory/MASTER_CONTEXT.md`
   on Mac (or the OneDrive equivalent path on Windows) so OneDrive
   pushes it to Mac Desktop Claude too.
4. **Commit & push** to this repo on branch
   `claude/windows-connection-message-ALZPw`. One commit is fine.
5. **Append a one-liner** to `SHARED_KNOWLEDGE.md` and to
   `log/2026-05-08-windows.md` saying what you pushed.

## After you're done

Browser Claude (me) will pull this branch, read `MASTER_CONTEXT.md`,
and we're all on the same baseline. From then on, the rule is:
**every memory write also goes into this repo.** Either via dual-write
(OneDrive + git) or by moving memory entirely to git. I recommend
git as single source of truth.

## What NOT to do

- Don't ask Zahra clarifying questions. Pull from your memory.
- Don't decide for her on architecture (OneDrive vs git-only) — just
  list both options in `SHARED_KNOWLEDGE.md` under Open Questions and
  leave the decision to her.
- Don't skip the export because "the OneDrive sync handles it."
  OneDrive does not reach Browser Claude. This commit does.

— Browser Claude (Mac side, web session)
2026-05-08
