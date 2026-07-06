---
name: decide
description: Use when a pool of solution options exists and you need to select one, the Double Diamond's fourth move (Deliver, the solution-space narrow, which we call "decide"). Runs AFTER `develop` and hands off to `probe`. Also called (industry synonyms): deliver, converge, select, choose, narrow, prioritize, commit. Trigger on "decide", "converge", "pick one", "narrow it down", "which option", "choose an approach", "decide between these", Swedish "besluta", "konvergera", "välj en", "vilket alternativ". Selects ONE solution idea WITH the operator; it does not generate new options or write a spec.
---

# decide

The **fourth move** of the Double Diamond (design thinking): **Deliver**, the solution-space
**narrow**, which we call **decide** (it decides *which* solution to pursue, before anything is
built or shipped). Given a pool of solution options, narrow to **one** idea. It runs after `develop`
(which generated the pool) and hands the winner to `probe` (which tests its riskiest assumption
before it is specified). This is the **selection** phase the method deliberately keeps separate from
generation, so this is where judgment finally happens.

## Core principle

Narrow deliberately, with criteria, **with the operator**. Convergence is a workshop move:
**group, then vote, then pick**. After clustering (affinity), a **dot-vote** surfaces priorities
before any final decision. Voting informs; the operator still holds the final pick (a tally is not a
verdict). Being told "just decide for me" does not release the choice. The **dot-vote is a tool for
a genuine field of competing options**, offered to the operator, not a ritual to run on every
convergence. Stay a **thinking partner**: surface the discriminator and let the operator choose
(they may combine options); never announce "now we'll run the vote" and start driving a process the
operator didn't ask for. A lean is fine; a default-on-silence, or sliding straight into a spec, is
not, the chosen idea goes to `probe` next, not into a spec.

## Precondition

A solution **option pool** (`## Develop`) must exist in the working file (`discover` creates the
file in the working repo at `docs/designthinking/<slug>.md`, else `~/.claude/design/<slug>.md`,
gated by its `Status` field). Require `Status ≥ deciding`; if it is lower or the file is missing,
stop and point to `develop` (or `discover`/`define` if the problem isn't framed either).

## When to skip it

`decide` **selects one from an enumerable pool of mutually-exclusive whole-solution options.** If
that isn't the work, you're **building a model / taxonomy** or **co-developing a vocabulary** with
the operator one concept at a time, not choosing between competing wholes, then this is **not**
`decide`. Don't manufacture a fork or a dot-vote where none exists; say so and stay in the
operator-led build. (That collaborative-build mode is a known gap in these skills, not yet its own
move.)

## Workflow

1. **Read the pool and the defined problem** (`## Develop` and `## Define`) from the working file.
2. **Cluster (affinity).** Group the raw options into a handful of genuinely distinct approaches
   (merge rewordings, keep distinct mechanisms).
3. **Set criteria with the operator.** What actually decides this (cost, risk, reversibility, fit,
   speed)?
4. **Dot-vote (group → vote, as in a workshop).** Give the operator a dot budget (default 5) to
   distribute across the clusters/options, stacking allowed. Optionally fan out independent
   agent-voters, each casting the same budget under the agreed criteria, blind to each other; then
   tally, so selection also pulls from independent sources. Collect the operator's dots **first** so
   the panel tally never anchors them. The board narrows the field to a top-voted shortlist.
5. **Narrow to ONE.** The operator picks from the shortlist (combining is fine). You hold the pick
   and surface the tradeoff; the tally **informs, it does not decide**, and you never set a default
   he must veto.
6. **Write and hand off.** Write the `## Decide` section (criteria + vote tally + the one chosen
   idea), set `Status: probing`, and hand the single idea to `probe` to have its riskiest assumption
   tested before it is specified.

## Reset

If nothing in the pool fits, reset to `develop` for more options. If the criteria reveal the
**problem itself** is wrong, reset to `define` (or `discover`). Moving `Status` backward is the
method's iteration, not a failure.

## What it does NOT do

- **Doesn't generate new options** — that is `develop`; if the pool is thin, reset to it.
- **Doesn't decide for the operator** — it lays out the discriminator and holds the pick, even when
  told to decide.
- **Doesn't specify** — the chosen idea goes to `probe` (then `brainstorming`, once it passes);
  `decide` writes no spec, plan, or code.

## Common mistakes

| Mistake | Right |
|---------|-------|
| "Just decide for me" → pick one and start speccing | Hold the pick; surface the discriminator; hand off after the operator chooses |
| Manufacturing a default-on-silence | The choice stays with the operator |
| Generating fresh options here | Reset to `develop`; `decide` only selects |
| Sliding from the pick straight into a spec | Hand the one idea to `probe`; it tests before `brainstorming` specifies |
| Selecting on an empty/thin pool | Reset to `develop` (or `define`) |
| Jumping from clusters straight to a pick | Group, then dot-vote, then the operator picks from the top |
| Showing the panel tally before the operator votes | Collect the operator's dots first; don't anchor them |
| Running a dot-vote with no real field of competing options | If it isn't a selection among mutually-exclusive wholes, it isn't `decide`; bow out |
| Announcing "now we'll run X" and driving a process | Propose and surface the discriminator; the operator drives |
