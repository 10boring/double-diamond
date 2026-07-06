---
name: develop
description: Use when the problem is defined and you need to generate solution options for it, the Double Diamond's third move (Develop, the solution-space widen). Runs AFTER `define`, BEFORE `decide`. Also called (industry synonyms): ideate, generate, brainstorm, diverge, sketch, explore options, produce. Trigger on "develop options", "ideate", "generate options", "brainstorm approaches", "what are the approaches", "widen the solutions", Swedish "ta fram lösningar", "vilka lösningar finns", "divergera". Generates raw options with judgment deferred; it does NOT evaluate, rank, or pick.
---

# develop

The **third move** of the Double Diamond (design thinking): **Develop**, the solution-space
**widen**. Given a **defined** problem, generate solution options widely. It runs after `define`
(which framed the problem) and before `decide` (which selects). The method's central rule holds it
in place: **separate the generation of ideas from the selection of ideas**. `develop` only generates.

## Core principle

Widen the solution space, judgment **deferred**. `develop` produces a raw pool of distinct options
and attaches **no** evaluation to them. Real divergence pulls from **independent sources**: the
operator's own ideas (however crazy) and several parallel agents, each blind to the others, because
a list you generate alone carries one model's blind spots. Ranking, pros/cons, a discriminator, a
recommendation, or picking a winner all belong to `decide`; doing any of them here fuses generation
with selection, the one thing the method forbids.

## Precondition

A `## Define` problem statement must exist in the working file (`discover` creates the file in the
working repo at `docs/designthinking/<slug>.md`, else `~/.claude/design/<slug>.md`, gated by its
`Status` field). Require `Status ≥ developing`; if it is lower or the file is missing, stop and
point to `define` (or `discover` if the problem isn't grounded either).

## When to skip it

If the defined problem has only one real solution approach, say so and skip to `decide` (or
straight to specifying). Don't pad a settled solution into a fake option set.

## Workflow

1. **Read the defined problem** (`## Define`) from the working file. Develop on *that*, not on the
   raw ask.
2. **Generate from independent sources**, operator first so you don't anchor:
   - **Operator first.** Ask for the operator's own solution ideas and explicitly invite the wild
     ones.
   - **Parallel agents.** Dispatch 3–4 subagents at once, each from a distinct lens (invert/kill
     the premise, cross-pollinate from other tools and domains, maximally-ambitious/unconstrained),
     blind to each other; collect and dedup. (If parallel agents aren't available, run the lenses
     yourself sequentially, each a separate blind pass.) Agents give **breadth, not proof**, their
     agreement is not validation.
   - **Your own pass**, as one more contribution, not the frame.
3. **List the pool raw, judgment deferred.** Keep genuinely distinct options (different in mechanism
   or shape, not a knob turned), including at least one that challenges the framing. "Dedup" and
   "distinct" mean **collapse restatements of the same mechanism only**; never cull an option for
   being weak, risky, or unlikely, that judgment is `decide`'s. Give each a name and a one-line
   essence, and **nothing else**: no why-it-wins, no risk, no ranking, no lean.
4. **Write and hand off.** Append the `## Develop` pool (unjudged) to the working file, set
   `Status: deciding`, and point to `decide`.

## Reset

If generating solutions reveals the problem is mis-defined, stop, say so, and reset to `define` (or
`discover`) — move `Status` back. A discovery sending you back to the problem is the method working,
not a failure.

## What it does NOT do

- **Doesn't evaluate, rank, or attach pros/cons** — judgment is deferred to `decide`.
- **Doesn't pick or recommend** — no winner, no lean, no default.
- **Doesn't specify** — produces options, not a brief.
- **Doesn't run on an undefined problem** — that is `define`'s output and this skill's precondition.
- **Doesn't generate from one context alone** — solicit the operator and fan out agents first.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Attaching "why it could win / main risk" to options | Generate raw; evaluation is `decide`'s job |
| Naming a discriminator or a lean | Defer all judgment; `decide` sets criteria and picks |
| Generating every option yourself from one context | Ask the operator (crazy welcome) and fan out agents |
| Three variants of one idea | Distinct mechanisms; at least one challenges the framing |
| Culling a "weak" option while deduping | Dedup merges restatements only; never drop on quality, that's `decide` |
| Developing on the raw ask | Develop on the defined problem from the working file |
| Padding a one-approach problem into fake options | Say there's one path; skip to `decide` |
