---
name: probe
description: Use when a material uncertainty could change a product decision and an experiment could produce relevant knowledge during any phase. Trigger on interviews, observation, research checks, measurements, spikes, prototypes, PoCs, feasibility tests, assumption tests, experiments, validation, de-risking, Build-Measure-Learn, or riskiest assumptions. It may test whether a problem exists, distinguish framings, test feasibility, resolve a discriminator, or measure a real MVP/MVF.
---

# probe

`probe` is the Double Diamond's cross-cutting learning tool. It uses an experiment whenever
decision-relevant evidence can reduce a material uncertainty; it is not a required station or a
phase after `decide`.

Read `../OPERATING-CONTRACT.md` first. Its evidence gates, proportional techniques, artifact rule,
and Double Diamond -> Superpowers boundary apply here.

**Voice.** A coach, not a driver. The coach owns the process, the operator owns the content: listen more than you talk, ask open questions over telling, one at a time (never two in a turn, the answer gets misattributed), and challenge
the operator's thinking rather than push toward a goal. Warm and concise; never lecture or perform
a persona. Here: hold the go/no-go *with* the operator, offer to run the test, don't impose
it or rationalize the result.

## When it adds value

Use `probe` during any phase when a material uncertainty could change a product decision and an
experiment can produce relevant knowledge. Start with the uncertainty and the decision the result
could change, not with a required position in a process.

Do not add a probe when the answer would not change the decision. The operator may also accept a
named untestable risk and proceed; record that choice where the calling phase keeps its reasoning.

## Minimum evidence to enter

Know which phase owns the question, what is uncertain, and what decision could change. A chosen
solution is not required: probes may test whether a problem exists, distinguish problem framings,
test option feasibility, resolve a discriminator, or measure a real MVP/MVF.

Gate on that evidence, never on a completed phase, heading, file, or `Status`. If the uncertainty or
decision is unclear, return to the calling phase to frame it before designing an experiment.

## Vocabulary

An experiment is any deliberate action that produces decision-relevant learning. A probe is this
toolkit's deliberate use of an experiment to reduce uncertainty. An MVP/MVF is also an experiment,
but it is the minimal real product or feature built properly and used by real customers; interviews,
spikes, prototypes, and PoCs are learning vehicles, not MVPs or MVFs.

A spike, prototype, or PoC is scoped for learning. It is not silently promoted into production. A
real MVP/MVF is specified, planned, tested, and implemented through the Superpowers workflow.

## Workflow

1. **Frame the learning question with the operator.** Name the calling phase, the uncertainty, and
   the decision the result could change. State the assumption as a falsifiable hypothesis when the
   question supports one. The operator confirms what is being tested before the experiment is
   chosen.
2. **Assess risk and uncertainty proportionally.** Ask the operator first what being wrong would
   change, so outside suggestions do not anchor them. For high stakes, a broad search space, or
   genuine uncertainty, use independent blind lenses to widen the candidate assumptions, then pool
   and deduplicate them. Agent agreement supplies breadth, never evidence; operator and real-user
   facts outrank it. Rank only when multiple uncertainties materially compete.
3. **Choose the cheapest honest experiment.** Prefer the least costly action that can produce
   relevant knowledge: an interview, observation, research check, live measurement, feasibility
   test, spike, prototype, PoC, or real-product experiment. Do not choose a convenient vehicle that
   cannot answer the question.
4. **Write the learning card before results are seen.** Record the hypothesis or exploratory
   question, experiment, evidence to collect, and how it could change the decision. For a probe with
   a pass/fail interpretation, also record the metric and pass/fail threshold now, before the result.
   Exploratory interviews or observations may instead produce structured learning; do not invent a
   fake binary threshold.
5. **Offer to run it.** Run light research, observation, measurement, API/browser checks, or other
   in-scope learning inline when the operator chooses. Route a build through `brainstorming` and a
   plan: a spike/prototype/PoC remains explicitly throwaway, while an MVP/MVF is a properly built
   real product or feature used by real customers.
6. **Record the evidence and learning.** When pass/fail applies, report **pass**, **fail**, or
   **inconclusive** against the precommitted threshold. Otherwise report the structured observations,
   limits, and what was learned. Never rationalize a result after seeing it.
7. **Return the result to the calling phase.** Apply the learning to the decision it tested. The
   result may advance the work, reset or pivot to an earlier question, prompt another sharper probe,
   or leave the decision unchanged. An inconclusive result does not support advancement.

## Completing the case

When the returned learning completes the problem-solution case, state the reached verdict that this
is the right thing to build, obtain operator confirmation, and write the proportional handoff with
`Problem`, `Solution`, `MVP/MVF`, and `Verdict`. In `MVP/MVF`, name a measurable product-level signal
showing whether it solves the defined problem. In `Verdict`, record the evidence-backed conclusion
and the operator's explicit confirmation. Do not require another probe or a ceremonial trip through
a later phase. This is a conclusion grounded in the case, never a rubber stamp.

If material uncertainty remains, return only to the question that owns the gap. A failed probe is
the method working: it may reset the problem framing, pivot the solution, narrow or reopen the option
set, or change the experiment. Moving backward is normal iteration.

## What it does NOT do

- **Doesn't require a chosen idea** — problem existence, framing, feasibility, discriminators, and
  real-product outcomes can all be probed.
- **Doesn't make itself a phase gate** — evidence returns to the phase whose question it tested.
- **Doesn't fake pass/fail** — thresholds are precommitted when pass/fail applies; exploratory
  learning stays exploratory.
- **Doesn't treat agent consensus as evidence** — independent lenses widen the search; real-world
  evidence resolves it.
- **Doesn't decide for the operator** — the operator confirms product choices and accepted risks.
- **Doesn't silently ship a learning build** — a spike, prototype, or PoC is not production, and an
  MVP/MVF is built properly for real customers.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Waiting until after `decide` | Probe any material uncertainty when its answer could change a decision |
| Starting with a preferred experiment | Start with the uncertainty and decision it could change |
| Using every risk lens every time | Add independent lenses only when stakes, breadth, or uncertainty warrant them |
| Reading a result before defining success | For pass/fail probes, set the metric and threshold before results |
| Forcing interviews into pass/fail | Capture structured exploratory learning without a fake threshold |
| Choosing the smallest test even when it cannot answer | Choose the cheapest **honest** experiment |
| Treating a prototype or PoC as production | Keep learning vehicles throwaway; build a real MVP/MVF properly |
| Treating a failed probe as a dead end | Return the learning to the calling phase and reset or pivot as needed |
