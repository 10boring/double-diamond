---
name: probe
description: Use when an idea has been chosen but its riskiest assumption is untested, the Lean Build-Measure-Learn step added onto the Double Diamond (beyond the four D's discover/define/develop/decide; the operator may call it an experiment). Runs AFTER `decide` and BEFORE superpowers `brainstorming`. Also called (industry synonyms): experiment, validate, test, prototype, de-risk, Build-Measure-Learn, riskiest-assumption test. Trigger on "probe", "experiment", "validate the idea", "test the assumption", "de-risk this", "riskiest assumption", "before we spec it", "will this actually work", Swedish "testa antagandet", "experiment", "avriska", "innan vi specar". Designs the cheapest experiment that could disprove the riskiest assumption AND offers to run it; light recon/measurement runs inline, only a real product build routes out; it does not write a spec.
---

# probe

The **fifth move**, the Lean **Build-Measure-Learn** step added onto the Double Diamond (design
thinking): the four D's end at `decide`; `probe` de-risks the chosen idea before it is specified. It
runs after `decide` (which selected the idea) and before superpowers `brainstorming` (which
specifies it). Pure design thinking stops at Deliver; `probe` makes the Lean validate loop explicit
(the operator may call a probe an *experiment* — same thing). The rule that holds it in place: **an
experiment must be able to fail**, and its pass/fail threshold is set **before** the result is seen.

## Core principle

De-risk the pick before you spec it. `probe` finds the assumption most likely to kill the chosen
idea and designs the **cheapest honest experiment** of it, with judgment fixed **in advance**: the
pass/fail threshold is written down before the experiment runs, so the result can't be rationalized
after the fact.

**`probe` designs the experiment AND offers to run it.** Design and execute don't cleanly separate
here, and pretending they do is a mistake. Light recon and measurement — desk research, a quick
`curl`, an API call, a driven browser session, a web search, a concierge / Wizard-of-Oz / fake
door — run **inline**; offer to run them whenever you can, the operator decides how. Only a *real
product build* routes out, to `brainstorming` → plan as a scoped, **throwaway** validation build
that gets its own scope-gate so it can't silently become the product.

**An experiment is not the product.** A probe is a throwaway test of one assumption. The *pipeline*
terminates one level further out, in a **minimal viable deliverable** — an **MVP** (minimal viable
product) for a whole product, an **MVF** (minimal viable feature) for a feature. That minimal
deliverable is the first *real* thing shipped to real users, and it doubles as the big
Build-Measure-Learn probe — but it is a product/feature, built via `brainstorming` → plan →
implement, never a throwaway experiment. Don't conflate the two.

## Precondition

`probe` de-risks a chosen idea, so the gate reads the whole upstream chain for **genuine content**
in the working file (`docs/designthinking/<slug>.md`, else `~/.claude/design/<slug>.md`):

- `## Discover` — real problem material;
- `## Define` — a reframed problem **the operator confirmed**, plus the named smuggled assumption;
- `## Develop` — a pool of distinct options;
- `## Decide` — the one **chosen idea**.

`Status` is a breadcrumb for the reader, never the gate: a hand-set `Status:` line proves nothing;
the content and the operator's confirmation do.

<HARD-GATE>
No probe without a real chosen idea sitting on a real, operator-confirmed `## Define`. If the chain
is missing a link, back up to the phase that's actually empty (→ `decide`, or `develop`/`define`/
`discover` if the gap is further up) — moving `Status` back is the method working, not a failure.

Two things this gate deliberately *does* let through, because backing into a skipped phase is
legitimate iteration, not an error:
- `Status: ready-to-specify` but no `## Probe` was ever run — `decide` handed straight to a spec and
  skipped this move. Back `Status` to `probing` and run.
- Re-running a probe already done.

Stepping over on purpose is allowed too — the operator may accept a named untestable risk and
proceed — but only consciously and **on record** in `## Probe`. Only the *accidental* skip is
blocked.
</HARD-GATE>

## When to skip it

High bar by design, because the failure this move prevents is skipping validation too eagerly. Skip
only when **no assumption is both high-risk and uncertain** (nothing a cheap experiment would
change), or the operator **explicitly accepts a named untestable risk** and it is recorded in
`## Probe`. Being told "just build it" does not release the gate; the operator may still knowingly
proceed on an unvalidated bet, recorded as such.

## Workflow

1. **Read the chosen idea and the surfaced assumptions** from `## Decide` and `## Define`.
   `discover`/`define` and `decide` already surfaced the assumptions and the discriminator, reuse
   them; do not re-discover.
2. **Rank the assumptions by risk × uncertainty**, from independent sources, operator first so you
   don't anchor:
   - **Operator first.** Ask what, if it turned out false, would kill the idea.
   - **Parallel agents.** Fan out 3–4 subagents to **red-team**, each blind to the others, on "the
     thing most likely to kill this idea is X"; pool and dedup. (If parallel agents aren't
     available, run the lenses yourself sequentially, each a separate blind pass.)
   - **Agent agreement is breadth, not evidence.** Four LLMs share priors, so a unanimous panel can
     be confidently wrong; a single operator or real-user fact outranks it. Use the agents to
     *widen* the candidate assumptions, never to *validate* one.
   - The **riskiest** = highest risk × highest uncertainty. Drop what is already known-true or
     low-stakes.
3. **Confirm the assumption's framing with the operator, then write the test card** into `## Probe`.
   The first framing is often architecturally naive — you may be about to test the wrong thing — so
   have the operator confirm *what* is being tested before you commit the card:
   - **Hypothesis** — the assumption stated so it can be false.
   - **Cheapest honest experiment** — prefer **zero-build** (desk research, concierge / Wizard-of-Oz,
     fake door, a measurement against a live source); only if none can answer it, a scoped throwaway
     build handed to `brainstorming` → plan.
   - **Metric** — what the experiment measures.
   - **Pass/fail threshold, written now, before it runs.**
4. **Offer to run it; run what you can; record what you find.** Run inline whatever you can
   (recon, measurement, API calls, a driven browser). Route only a *real product build* out to
   `brainstorming` → plan (throwaway, scope-gated). Record the result in `## Probe` as you go — the
   working file is a **living document**, revise it in place rather than only stacking new layers.
5. **Record the verdict** in `## Probe` (pass / fail / inconclusive + the learning) and branch:
   - **Pass** → set `Status: ready-to-specify`; the idea goes to `brainstorming` → plan → implement
     to build the **MVP / MVF** (the minimal viable deliverable that doubles as the big probe).
   - **Fail** → move `Status` back to `discovering` or `developing` with the learning; the idea, the
     framing, or the option set was wrong.
   - **Inconclusive** → design a cheaper or sharper experiment; don't spec on an unresolved bet.

## Reset

A failed probe is the method working: it sends you back to `develop` (wrong idea) or `discover` /
`define` (wrong problem) with a learning you didn't have before. Moving `Status` backward is
iteration, not failure.

## What it does NOT do

- **Doesn't build the product / MVP / MVF** — the minimal deliverable is built *after* a pass, via
  `brainstorming` → plan → implement; a probe's own throwaway validation build (if any) is
  scope-gated and never becomes the product.
- **Doesn't treat agent consensus as evidence** — a unanimous panel is breadth; operator/user data
  outranks it.
- **Doesn't decide for the operator** — it surfaces the riskiest assumption and holds the go/no-go;
  the operator may accept a named untestable risk and proceed, recorded.
- **Doesn't specify** — the chosen idea goes to `brainstorming` only after a pass; `probe` writes
  no spec, plan, or code.
- **Doesn't rank from one mind** — solicit the operator and fan out blind red-team agents first.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Speccing straight after `decide` | Probe the riskiest assumption first |
| An experiment that can only confirm | It must be able to fail |
| Reading the result, then deciding what "pass" meant | Threshold set before it runs |
| Refusing to run a cheap test you could run | Offer to run it inline; only a real product build routes out |
| Treating a unanimous agent panel as validation | Agent agreement is breadth; operator/user data outranks it |
| Writing the card before confirming what's tested | Confirm the assumption's framing with the operator first |
| Building the MVP and calling it "the probe" | The probe tests one assumption cheaply; the MVP/MVF comes after, via plan → implement |
| Calling the MVP a throwaway experiment (or vice versa) | An experiment is a throwaway test; the MVP/MVF is the minimal *real* deliverable |
| Skipping probe because it "obviously works" | Skip only if nothing is high-risk AND uncertain |
