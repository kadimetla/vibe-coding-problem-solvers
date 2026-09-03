# Alternative deck — story spine (v6)

**Not the official deck.** The official one is still `presentation/presentation-v3-marp.md`.
This is a candidate rebuild, kept here for comparison after the next live session.

## What it is

32 slides built around six true build stories instead of a list of techniques.

Spine: **Notice → Ask → Look → Keep or kill.** Stated at slide 3, demonstrated by every story,
repeated as a takeaway card at the end.

The six stories, in escalating ambition:

| # | Story | Beat it teaches |
|---|---|---|
| 1 | Pressroom — photos printed four to a page | One plain sentence is often enough |
| 2 | Quiz app — 17 months, still open | The keepers announce themselves |
| 3 | Image triage → file triage | Your second tool is your first one, generalised |
| 4 | Video note taker — timestamped notes | Small motions are the best candidates |
| 5 | Escócia '26, rebuilt from the Iceland version | Cheap to make means cheap to throw away |
| 6 | Lisbon Olympics — a whole tournament | Automate the bottleneck, not the event |

Story 6 is told, not walked through. It's framed as the deep end you arrive at, not where you start.

## Build it

```bash
npx @marp-team/marp-cli@latest \
  --config ~/.claude/skills/marp-slides/.marprc.yml \
  --theme-set ~/.claude/skills/marp-slides/assets/brand \
  --html --no-stdin presentation-v6.md -o presentation-v6.html
```

Add `--allow-local-files` for the PDF. Live editing: `~/.claude/skills/marp-slides/scripts/marp-live.sh presentation-v6.md`
(that embeds a reload client — re-export without `--watch` before shipping).

## Images

`img/` holds three kinds:

- **Generated plates** (`01-instrument`, `07-promote`, `s1-the-motion`, `s2-handing-it-over`) — risograph
  illustrations made with the OpenAI imagegen skill, prompted to the `automata` palette.
- **App screenshots** (`app-*`) — real captures. Pressroom and Scotland were captured live; quiz, file
  triage and video notes come from `assets/screenshots-v3/`.
- **Olympics captures** (`oly-*`) — captured by running `apps/lisbon-olympics-2026` locally with the
  Supabase env vars cleared, which makes the store fall back to in-memory. The hosted Supabase project
  no longer resolves, so the original event data is gone. Roster and times in these shots are demo data.

## Status

Pending review after the next live delivery. Open questions carried over:

- How many stories survive contact with a real audience
- Whether the decision-deck demo comes back (it was dropped here)
- Which parts of the v3 deck's technique material to fold back in

See `vibe coding course v6 alternative deck` and `vibe coding course v4 deck rationale` in the vault.
