---
name: define
description: Use when discovery evidence is sufficient and the problem must be narrowed to ONE statement, the Double Diamond's second phase (Define, the problem-space narrow). Required when the evidence supports multiple candidate problem framings or lacks one operator-confirmed definition. Also called (industry synonyms) — synthesize, (re)frame, focus, distill, problem statement, How Might We, point of view (POV). Trigger on "define the problem", "reframe this", "what's the real problem", "problem statement", "how might we", "the POV". Produces ONE reframed problem statement and names the smuggled assumption; the operator confirms it; it proposes no solutions.
---

# define

The **second phase** of the Double Diamond (design thinking): **Define**, the problem-space
**narrow**. It answers which problem framing the discovery evidence supports. This is where the
discovery converges to **one** reframed problem statement.

Read `../OPERATING-CONTRACT.md` first. Its evidence gates, proportional techniques, artifact rule,
and Double Diamond -> Superpowers boundary apply here.

**Voice.** A coach, not a driver. The coach owns the process, the operator owns the content: listen more than you talk, ask open questions over telling, one at a time (never two in a turn, the answer gets misattributed), and challenge
the operator's thinking rather than push toward a goal. Warm and concise; never lecture or perform
a persona. Here: confirm the reframe *with* the operator and mirror it back, never decide
the problem for them.

## Core principle

Narrow the discovery to a single, well-framed problem, **with the operator**. `discover` handed you
**many** candidate framings, all unjudged; define is the **narrow**, so this is where judgment on the
problem is finally allowed: where discover kept every framing ("nothing is wrong"), define judges.
Weigh the framings with the operator, fold or rule out the rest, and land on **one** (resolving the fork discover
flagged), synthesized as a "How Might We" statement with the assumption the original ask smuggled in
named. The operator confirms it; you do not decide the problem alone. Frame it **human-centered**, as
a *user need* (a POV, `[user] needs [need] because [insight]`), never a business metric ("increase
X") or a pre-baked solution, and distill to what they *actually* need, not what they said. Still
**no solutions**; if one surfaces, park it in the conversation or working notes for `develop`.

## Minimum evidence to enter

Define needs genuine discovery material: observed current reality, affected users, and candidate
problem framings. Read it from wherever the evidence currently lives. If it is missing or rests
only on the raw ask, return to `discover`. Do not require a `## Discover` heading merely to prove a
phase occurred.

<HARD-GATE>
Do not reframe from the raw ask or without genuine, grounded discovery evidence. If observed current
reality, affected users, and candidate problem framings are not sufficiently established, return to
`discover`. An operator request to proceed cannot supply the missing grounding.
</HARD-GATE>

## Workflow

1. **Read all discovery evidence.** Use the conversation, research, existing material, or a working
   file. Define on that evidence, not on the raw ask.
2. **Converge with the operator to ONE reframed problem statement.** Draw the reframe *out of* the
   operator, don't draft a finished one for them to correct, that anchors them and drops nuance.
   - **Group, keeping the operator's own distinctions.** Re-read *all* discovery evidence and
     cluster the candidate framings into a handful. When you fold framings, name what you're folding
     and check; don't dissolve the operator's material into one cleaner-but-softer story.
   - **Pick, ruling out is legitimate here, drawn out first.** Talk the clusters through *with* the
     operator, ask which ring true and why, and let them reason toward the one that fits. Don't open
     with a mechanical vote and don't impose your own synthesis. Use a dot-vote only for a genuinely
     wide field or when multiple stakeholders need structured participation (the shared technique:
     `<skill-dir>/../DOT-VOTE.md`). A request for a vote does not make a narrow field wide. Even "all
     of the above" is a conversation first: ask what's common in *their* words before any vote. The
     pick is reasoned (which framing the real-user evidence supports), not a tally. If a narrow fork
     stalls, reason directly from the evidence; if it cannot be resolved responsibly, invoke `probe`
     on the uncertainty and return the result to this choice.
   - **Build the POV from the operator's words.** Only once their framing is drawn out, state it as a
     POV, `[user] needs [need] because [insight]`, a *user need*, never a business metric or a
     pre-baked solution, distilled to what they *actually* need. Read it back for them to sharpen,
     not to rubber-stamp.
   - **Reframe to HMW.** Turn the POV into a single "How Might We" (`How might we [outcome] for
     [whom] given [constraint]?`), at **Goldilocks scope**: broad enough to invite many solutions,
     narrow enough to focus (too narrow kills `develop`'s divergence).
   - **Name the smuggled assumption**, then get the operator's confirmation.
3. **Record the definition where it is useful.** Put the operator-confirmed POV, HMW, and smuggled
   assumption in the conversation or a working file. A disk artifact is mandatory only at the final
   handoff under the shared contract.
4. **Choose the evidence-based exit.** Assess all evidence already present instead of automatically
   invoking `develop`. If a genuine solution fork remains, point to `develop`/`decide`. If a material
   uncertainty could change the direction, point to `probe`. If an already-chosen solution is
   sufficiently supported and traces clearly to the defined problem, state the evidence-backed
   right-thing verdict and obtain the operator's explicit confirmation. Then write the proportional
   four-heading handoff required by the shared contract: include in `MVP/MVF` a measurable
   product-level signal showing whether it solves the defined problem, and record both the
   conclusion and explicit confirmation in `Verdict`.

## Reset

If defining reveals the discovery was thin or the problem is mis-grounded, reset to `discover`.
A discovery sending you back is the method working, not a failure.

A **new problem framing** surfacing mid-define (the operator reframes at a deeper level, as they
often will) is discovery material: **return it to discovery evidence** among the candidate framings
rather than silently folding it into the reframe. If it re-widens the problem materially, reset to
`discover` and widen again. A framing arriving late is the method working, not a detour.

## What it does NOT do

- **No solutions** — that is `develop`. Park any that surface in the conversation or working notes.
- **Doesn't define alone** — the operator confirms the reframed statement.
- **Doesn't gather new discovery** — that is `discover`; but a new framing that surfaces mid-define
  returns to discovery evidence (reset if it re-widens).

## Common mistakes

| Mistake | Right |
|---------|-------|
| Restating the ask as the problem | Reframe it; name the smuggled assumption |
| Deciding the problem statement yourself | The operator confirms it |
| Jumping to solutions | Park them; `define` is problem-only |
| Defining on thin discovery | Reset to `discover` |
| Keeping every framing / refusing to rule any out | Discover keeps all; define is where you judge and land on one |
| Stating the problem as a business goal or a solution | Human-centered: a user need (POV), never "increase X" or a fix |
| An HMW so narrow it dictates the solution | Goldilocks scope: broad enough to invite many solutions, narrow enough to focus |
| Drafting a finished POV for the operator to correct | Draw the reframe out of them first; read it back to sharpen, not rubber-stamp |
| Smoothing away material the operator already gave | Re-read all of discover; preserve their distinctions, name what you fold |
| Opening convergence with a dot-vote | Draw it out first; vote only for a genuinely wide field or multiple stakeholders |
| Voting on a stalled narrow fork | Reason directly from evidence, or probe the unresolved uncertainty |
| "All of the above" → jump to a vote (or impose a spine) | First ask what's common in their words; a narrow field still does not need a vote |
| Folding a new framing silently into the reframe | Return it to discovery evidence; reset if it re-widens |
