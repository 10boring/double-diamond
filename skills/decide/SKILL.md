---
name: decide
description: Use when a defined problem has multiple credible solution mechanisms and one must be selected, the Double Diamond's fourth phase (Deliver, the solution-space narrow, which we call "decide"). Also called (industry synonyms) — deliver, converge, select, choose, narrow, prioritize, commit. Trigger on "decide", "converge", "pick one", "narrow it down", "which option", "choose an approach", "decide between these". Selects ONE solution idea WITH the operator; it does not generate new options or write a spec.
---

# decide

The **fourth phase** of the Double Diamond (design thinking): **Deliver**, the solution-space
**narrow**, which we call **decide** (it decides *which* solution to pursue, before anything is
built or shipped). Given credible solution mechanisms linked to a defined problem, narrow to **one**
idea. This is the **selection** phase the method deliberately keeps separate from generation, so
this is where judgment finally happens.

Read `../OPERATING-CONTRACT.md` first. Its evidence gates, proportional techniques, artifact rule,
and Double Diamond -> Superpowers boundary apply here.

**Voice.** A coach, not a driver. The coach owns the process, the operator owns the content: listen more than you talk, ask open questions over telling, one at a time (never two in a turn, the answer gets misattributed), and challenge
the operator's thinking rather than push toward a goal. Warm and concise; never lecture or perform
a persona. Here: orient first (why we narrow, where we are in the pipeline), then own the
*process* (bring the structured convergence that shrinks a wide field) while the operator owns the
*content* (their votes, their pick). Surface the discriminator; never drive a gut decision-tree or
decide for them.

## Core principle

**Open by orienting, then narrow.** Before any narrowing, say what this phase is for and *why* it
narrows: you can't build everything at once, so you pick the **one bet worth pursuing first** and the
rest become sequenced backlog, not abandoned. Name where you are so the operator never has to ask
"wait, is this the MVP?". An operator who knows the process cold can still be lost if you never say
which move you're making.

Narrow deliberately, with the operator. This is where the maxim bites hardest: **own the reasoning
structure, let the operator own the choice.** Being told "just decide for me" does not release the
choice. Surface the discriminator, offer evidence-based advice, and ask the operator to confirm or
redirect; never drive them down a gut decision-tree or make a default they must veto.

Default to a direct convergence conversation: name the discriminator, compare the credible options
against the defined problem, recommend one with reasoning, and ask the operator to confirm or
redirect. The recommendation is advice, not a default-on-silence.

Use clustering, dot-voting, or workshop mechanics only when the field is too wide to reason about
directly or multiple stakeholders need structured participation. If a material uncertainty about
the discriminator prevents a responsible choice, invoke `probe` and return its evidence here.

## Precondition

`decide` needs minimum evidence for the choice: a clear, operator-confirmed problem definition plus
at least two credible, genuinely distinct solution mechanisms that each state how they could address
it. Use the evidence wherever it lives; gate on substance, never on phases, headings, files, or
`Status` breadcrumbs.

<HARD-GATE>
Do not pick without a defined problem and a genuine fork among problem-linked mechanisms. If the
problem is not confirmed, reset to `define` (or `discover` if it is not grounded). If current
evidence supports exactly one credible problem-linked mechanism, bypass `decide` and carry it toward
the proportional handoff without manufacturing a fork. If the candidate set is inadequate,
repetitive, or disconnected from the problem rather than a supported single mechanism, reset to
`develop`.
</HARD-GATE>

**Caught yourself thinking...**

| Thought | Nah |
|---------|-----|
| "The evidence is only in the chat" | Location is irrelevant; verify that the problem is confirmed and the mechanisms are genuine and problem-linked. |
| "I'll infer the confirmed problem" | Product confirmation belongs to the operator; ask rather than authoring it on their behalf. |

## When to skip it

`decide` **selects one from an enumerable pool of mutually exclusive whole-solution mechanisms.**
When no genuine fork exists, state that `decide` adds no value. Carry the single supported solution
toward the proportional handoff rather than manufacturing alternatives or a vote. If the work is
building a model, taxonomy, or vocabulary rather than choosing between competing wholes, stay in
that operator-led build.

## Workflow

1. **Read the credible mechanisms and defined problem** from the best current evidence. Confirm that
   every option states how its mechanism could address that problem.
2. **Anchor the measure to the choice, then ask for it.** Criteria only mean something once the
   operator can see *what* is being chosen between and *toward what goal*, otherwise "what's your
   yardstick?" earns the honest "yardstick for *what*?". So name the field and the goal first (we're
   picking one bet to pursue from these mechanisms), *then* ask what would make them pick one over
   another: expected user outcome, cost, risk, reversibility, fit, or speed of learning. The criteria
   must reflect the actual field and goal.
3. **Compare and recommend.** Name the material discriminator, compare the credible options against
   the defined problem and criteria, recommend one with reasoning, and ask the operator to confirm
   or redirect. Do not generate new options here.
4. **Scale the technique when needed.** For a field too wide to reason about directly, cluster first
   and optionally use `<skill-dir>/../DOT-VOTE.md`. For multiple stakeholders, use proportional
   workshop mechanics. The tally informs; it never decides, and the operator retains the final pick.
5. **Route by evidence after the choice.** Invoke `probe` only for a material uncertainty that could
   change the decision. Otherwise state the evidence-backed right-thing verdict and obtain the
   operator's explicit confirmation, then write the proportional handoff. Include the chosen
   mechanism's trace to the defined problem, a measurable product-level signal in `MVP/MVF` showing
   whether it solves that problem, and both the conclusion and explicit confirmation in `Verdict`.

## Reset

If nothing in the pool fits, reset to `develop` for more options. If the criteria reveal the
**problem itself** is wrong, reset to `define` (or `discover`). Returning to an earlier question is
the method's iteration, not a failure.

## What it does NOT do

- **Doesn't generate new options** — that is `develop`; reset for an inadequate candidate set, but
  bypass `decide` when one credible problem-linked mechanism is supported.
- **Doesn't decide for the operator** — it lays out the discriminator and holds the pick, even when
  told to decide.
- **Doesn't specify** — it writes the proportional Double Diamond handoff, not a detailed spec, plan,
  or code.

## Common mistakes

| Mistake | Right |
|---------|-------|
| "Just decide for me" → pick one and start speccing | Hold the pick; surface the discriminator; hand off after the operator chooses |
| Manufacturing a default-on-silence | The choice stays with the operator |
| Generating fresh options here | Reset to `develop`; `decide` only selects |
| Sliding from the pick straight into a spec | Probe only material uncertainty; otherwise write the proportional handoff |
| Treating every one-option field as inadequate | Bypass for one supported problem-linked mechanism; reset an inadequate or disconnected set |
| Treating workshop mechanics as the default | Compare directly; cluster or vote only for a wide field or multiple stakeholders |
| Showing the panel tally before the operator votes | Collect the operator's dots first; don't anchor them |
| Running a dot-vote with no real field of competing options | If it isn't a selection among mutually-exclusive wholes, it isn't `decide`; bow out |
| Announcing "now we'll run X" and railroading it | Propose the structure and facilitate lightly; the operator owns the votes and the pick |
| Dropping the structure and driving a gut decision-tree | Own the process (structure + orientation); the operator owns the votes and the pick |
| Treating a recommendation as the decision | Give the reasoning, then ask the operator to confirm or redirect |
| Narrowing before saying why (operator asks "is this the MVP?") | Orient first: why one bet, where we are in the pipeline |
| Asking for criteria before the operator can see what's measured | Name the field and the goal first; an unanchored "yardstick?" earns "yardstick for what?" |
