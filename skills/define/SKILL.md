---
name: define
description: Use when discovery is done and the problem must be narrowed to ONE statement, the Double Diamond's second move (Define, the problem-space narrow). Runs AFTER `discover`, BEFORE `develop`. Also called (industry synonyms): synthesize, (re)frame, focus, distill, problem statement, How Might We, point of view (POV). Trigger on "define the problem", "reframe this", "what's the real problem", "problem statement", "how might we", "the POV", Swedish "definiera problemet", "rama in problemet". Produces ONE reframed problem statement and names the smuggled assumption; the operator confirms it; it proposes no solutions.
---

# define

The **second move** of the Double Diamond (design thinking): **Define**, the problem-space
**narrow**. It runs after `discover` (which widened on the problem) and before `develop` (which
generates solutions). This is where the discovery converges to **one** reframed problem statement.

## Core principle

Narrow the discovery to a single, well-framed problem, **with the operator**. Synthesize the
discovery into one "How Might We" statement and name the assumption the original ask smuggled in.
The operator confirms it; you do not decide the problem alone. Still **no solutions**, if one
surfaces, park it for `develop`.

## Precondition

A `## Discover` section must exist in the working file (`discover` creates it in the working repo
at `docs/designthinking/<slug>.md`, else `~/.claude/design/<slug>.md`, gated by its `Status`
field). Require `Status ≥ defining`; if it is lower or the file is missing, stop and point to
`discover`.

## Workflow

1. **Read `## Discover`** from the working file. Define on *that*, not on the raw ask.
2. **Converge with the operator to ONE reframed problem statement.** Synthesize into a single "How
   Might We" statement (`How might we [outcome] for [whom] given [constraint]?`), and name the
   assumption the original ask smuggled in. The operator confirms it.
3. **Write and hand off.** Write the `## Define` section (reframed statement + surfaced
   assumptions), set `Status: developing`, and point to `develop`.

## Reset

If defining reveals the discovery was thin or the problem is mis-grounded, reset to `discover`
(move `Status` back). A discovery sending you back is the method working, not a failure.

## What it does NOT do

- **No solutions** — that is `develop`. Park any that surface.
- **Doesn't define alone** — the operator confirms the reframed statement.
- **Doesn't gather new discovery** — that is `discover`; reset to it if the material is thin.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Restating the ask as the problem | Reframe it; name the smuggled assumption |
| Deciding the problem statement yourself | The operator confirms it |
| Jumping to solutions | Park them; `define` is problem-only |
| Defining on thin discovery | Reset to `discover` |
