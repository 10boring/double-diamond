---
name: guide
description: The Double Diamond front door — orientation across the five moves (discover → define → develop → decide → probe). Use when someone asks what double-diamond or the five skills do, where to start on a design decision, which move they're in, or what the next move is. Trigger on "what is double-diamond", "how do the five skills fit", "where do I start on this design decision", "which move am I in", "what's the next move", "help with double-diamond", Swedish "vad är double-diamond", "vilket steg/move är jag i", "var börjar jag på designbeslutet", "vad är nästa steg i designen". It orients and points to the one due move; it runs no move itself, and it bows out when no Double Diamond design decision is actually in play.
---

# guide

The **front door** to the Double Diamond. It orients: it senses where you are across the five moves
— **discover → define → develop → decide → probe** — names the move you're in and the one due next,
and points you at the right skill. It is the map, not a move; it discovers, defines, develops,
decides, and probes **nothing** itself.

## When this is NOT your call (bow out first)

Before anything else, check that a **Double Diamond design decision** is actually in play. Signals:
an existing working file at `docs/designthinking/<slug>.md` (or `~/.claude/design/<slug>.md`), or
the operator explicitly framing a *design* decision — what to build, which problem to solve, which
approach to take.

If none of that is present — the operator is mid-research-case, mid-implementation, asking a code
question, or using another tool that also has a "where are we?" front door (e.g. research-kit's
`guide`) — then **this is not the Double Diamond's question to answer.** Say so in one line and
stop. Do **not** default to "start at discover". "Where do we stand?" inside a research case is that
tool's call, not this one's. Speak only when the design-thinking process is genuinely the thing in
play.

## What it does

1. **Sense where you are.** If a working file exists, read the *content* of its `## ` sections, not
   the `Status` word (a hand-set `Status:` proves nothing — the gates read content, so does this).
   The furthest section carrying genuine content **and the operator's confirmation** is where you
   actually are.
2. **Name the move and the next.** Tell the operator the current move and the one due next, in the
   fixed order discover → define → develop → decide → probe, then out to superpowers `brainstorming`
   once `probe` passes.
3. **Point, don't do.** Hand off to the one due skill and stop.

## Where to start (only when a design decision IS in play)

- **No working file, problem not grounded** → `discover`.
- **No file, but the problem is already grounded and agreed in one sentence** → `define`.
- **An unframed pool exists** (options with no operator-confirmed `## Define` above them) → back to
  `define`; a pool without a framed problem isn't ready to decide. This is the exact skip the phase
  gates block — the guide names it early instead of letting it reach `decide`.
- **Otherwise** → the move after the furthest section that carries real, operator-confirmed content.

## The five moves (read them live)

Describe the five from their own skill descriptions and `README.md`, so this never goes stale:
**discover** (widen on the real problem), **define** (narrow to one framed problem + named smuggled
assumption), **develop** (widen on solutions, judgment deferred), **decide** (narrow to one idea
with the operator), **probe** (the cheapest experiment that could disprove the idea's riskiest
assumption). Generation and selection stay separate; the pipeline is iterative — any move can reset
to an earlier one, which is the method working, not a failure.

## What it does NOT do

- **Doesn't run a move** — it orients and points; the five moves are the other skills.
- **Doesn't answer for another tool** — no Double Diamond design decision in play, it bows out.
- **Doesn't trust the `Status` word** — it reads section content, like the gates do.
- **Doesn't decide, define, or generate** — zero convergence or divergence of its own.
