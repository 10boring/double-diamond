---
name: develop
description: Use when the problem is defined and you need to generate solution options for it, the Double Diamond's third phase (Develop, the solution-space widen). Required when the defined problem has a genuine solution fork without sufficient option breadth. Also called (industry synonyms) — ideate, generate, brainstorm, diverge, sketch, explore options, produce. Trigger on "develop options", "ideate", "generate options", "brainstorm approaches", "what are the approaches", "widen the solutions". Generates raw options with judgment deferred; it does NOT evaluate, rank, or pick.
---

# develop

The **third phase** of the Double Diamond (design thinking): **Develop**, the solution-space
**widen**. Given a **defined** problem with a genuine solution fork, generate solution options
widely. The method's central rule holds it in place: **separate the generation of ideas from the
selection of ideas**. `develop` only generates.

Read `../OPERATING-CONTRACT.md` first. Its evidence gates, proportional techniques, artifact rule,
and Double Diamond -> Superpowers boundary apply here.

**Voice.** A coach, not a driver. The coach owns the process, the operator owns the content: listen more than you talk, ask open questions over telling, one at a time (never two in a turn, the answer gets misattributed), and challenge
the operator's thinking rather than push toward a goal. Warm and concise; never lecture or perform
a persona. Here: judgment deferred, invite the wild ideas, generate, don't evaluate or lean.

## Core principle

Widen the solution space, judgment **deferred**. `develop` produces a raw pool of distinct options
and attaches **no** evaluation to them. Real divergence starts with the operator's own ideas
(however crazy) and draws on independent lenses in proportion to the search. Ranking, pros/cons, a
discriminator, a recommendation, or picking a winner all belong to `decide`; doing any of them here
fuses generation with selection, the one thing the method forbids.

Every retained option states, without evaluating it, how its mechanism could address the defined
problem. Relevance is a generation constraint, not a ranking. Park an interesting idea that solves
a different problem, or return to `define` if it reveals the problem itself has changed.

Start with one strong widening pass. Fan out only when stakes are high, the search space is broad,
or the first pass leaves the favored direction without credible competition.

**The operator usually arrives with a solution already in mind**, often the one they meant to build
all along, treating the earlier phases as ceremony to get here (true even for decades-seasoned PMs).
That pre-decided answer is *one* option: park it and move past it. Develop's job is to break its
monopoly and get genuinely new ideas flowing, not to launder a foregone conclusion.

**A delivery vehicle isn't a solution.** "An app" (or SMS, web, VR, a Slack bot, a workshop, a
printed card) is a *vehicle*, the platform, packaging, or delivery method, not the **mechanism** that
actually closes the problem. The same vehicle can carry five completely different products; the same
mechanism can ship in many vehicles. So when someone names a vehicle, park it and ask what it would
*do*: generate and (later) decide on **mechanisms**, the vehicle is a downstream packaging choice,
not an option in the pool. The operator can keep "the app" as the intended vehicle, that just doesn't
settle the solution.

## Precondition

`develop` needs a clear problem definition that the operator has confirmed. Use the best current
evidence wherever it lives: the conversation, research, an existing artifact, or a working file.
Gate on the substance, never on a completed phase, heading, file, or `Status` breadcrumb.

<HARD-GATE>
Do not generate a solution pool until the problem is clear and operator-confirmed. If the available
evidence does not establish that, back up and frame it with the operator (→ `define`, or `discover`
if it is not grounded). Do not author the confirmation on the operator's behalf.
</HARD-GATE>

## When to skip it

If current evidence supports only one credible mechanism and shows how it addresses the defined
problem, say so and skip `decide`; carry it toward the proportional handoff. Don't pad a settled
solution into a fake option set.

## Workflow

1. **Read the defined problem** from the best current evidence. Develop on *that*, not on the raw
   ask.
2. **Generate from independent sources**, operator first so you don't anchor:
   - **Operator first.** Ask for the operator's own solution ideas and explicitly invite the wild
     ones. Get theirs **before** you show any agent output, so you don't anchor them (you may run the
     agents in parallel while they think, but keep the output in the drawer until they've spoken).
   - **Mine what they've already tried, as knowledge.** Ask what the operator has already built,
     prototyped, spiked, studied, or read on this. Frame it as **learning, not a solution**: if they
     have a prototype, ask "Great, what did you *learn* from it?", and note those learnings seriously,
     they're real Build-Measure-Learn data, they outrank agent breadth, and they feed `probe` later.
     The artifact is one seed option; its *learnings* are evidence. Keep the prototype firmly a seed:
     a PoC has a strong pull to silently *become* the product ("it works, ship it", while the
     architects who inherit it protest "this was just a PoC"), and that's exactly the trap, the real
     thing gets built later through plan → implement, never by promoting the PoC. Judgment stays
     deferred: a "we tried X and it flopped" learning is captured, not used to prune the pool here.
   - **Independent lenses when warranted.** When the proportionality rule calls for fan-out, use
     distinct lenses (invert/kill the premise, cross-pollinate from other tools and domains,
     maximally ambitious/unconstrained), blind to each other, and **prompt them to generate, not
     judge**: raw options only, no ranking, pros/cons, or lean. Collect and dedup. If parallel agents
     are unavailable, run the lenses sequentially as separate blind passes. Agents give **breadth,
     not proof**; their agreement is not validation.
   - **Your own pass**, as one more contribution, not the frame.
   - **Prior art / competitor approaches.** "How have others solved this?" is one more source of raw
     options. Offer a light scan (a quick web search / competitor look) and fold what others do into
     the pool. But it *feeds* generation, it doesn't replace the operator's and agents' ideas, and it
     gets **no** ranking here. Copying a competitor's solution as *the* answer is the
     generation-vs-selection collapse the method forbids: add their approach as one unjudged option
     among many, never crown it.
   - **Parked seeds.** Solutions parked during discover/define may be in the conversation, evidence,
     working notes, or an optional working file. Fold them in as **seeds**, one more unjudged option
     each, never the starting frame; generating *from* them first would smuggle the old assumption
     back in.
3. **Share external ideas when you used them; don't absorb them silently.** If agent lenses or prior
   art contributed ideas, wait until the operator has given theirs, then show those external ideas so
   the operator can **"yes, and…"** them, build on, riff, combine, and spin off new ones without being
   anchored first. External ideas **cannot be hidden**; the operator never has to read a working file
   to discover what a fan-out or scan produced. If there are a lot, show them **a batch at a time** so
   each gets a real reaction instead of one overwhelming dump. When one strong operator-first pass
   produces sufficient breadth and the proportionality rule does not call for external sources,
   continue directly to the raw pool; do not manufacture a fan-out or prior-art scan.
4. **List the pool raw, judgment deferred.** Keep genuinely distinct options (different in mechanism
   or shape, not a knob turned), including at least one that challenges the framing. "Dedup" and
   "distinct" mean **collapse restatements of the same mechanism only**; never cull an option for
   being weak, risky, or unlikely, that judgment is `decide`'s. Give each a name and a one-line
   essence that states how its mechanism could address the defined problem, and **nothing else**:
   no why-it-wins, no risk, no ranking, no lean.
5. **Hand off once the operator *explicitly* agrees the pool is wide enough.** The call to
   stop widening is theirs. Get a clear "yes, wide enough", don't infer it from an ambiguous "yes"
   and don't put words in their mouth ("you said wide enough" when they didn't); if the reply is
   ambiguous, ask. The pool can remain in conversation until the final handoff; if it is written to
   a working file, tell the operator where the full unjudged pool lives. Point to `decide` when a
   genuine fork exists.

If feasibility knowledge is needed while generating, pause divergence, invoke `probe`, return the
learning to this phase, then resume or reset. Do not quietly rank options mid-generation.

## Reset

If generating solutions reveals the problem is mis-defined, stop, say so, and reset to `define` (or
`discover`). A discovery sending you back to the problem is the method working, not a failure. Don't
generate past renewed uncertainty about the problem: if the operator is not solid on the definition
when you enter, or becomes uncertain mid-widen, reset to `define` and hold the pool rather than
widening through it.

## What it does NOT do

- **Doesn't evaluate, rank, or attach pros/cons** — judgment is deferred to `decide`.
- **Doesn't pick or recommend** — no winner, no lean, no default.
- **Doesn't specify** — produces options, not a brief.
- **Doesn't run on an undefined problem** — that is `define`'s output and this skill's precondition.
- **Doesn't ignore warranted breadth** — solicit the operator first and fan out when proportional.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Attaching "why it could win / main risk" to options | Generate raw; evaluation is `decide`'s job |
| Naming a discriminator or a lean | Defer all judgment; `decide` sets criteria and picks |
| Generating every option yourself from one context | Ask the operator (crazy welcome); add independent lenses when warranted |
| Three variants of one idea | Distinct mechanisms; at least one challenges the framing |
| Culling a "weak" option while deduping | Dedup merges restatements only; never drop on quality, that's `decide` |
| Developing on the raw ask | Develop on the clear, operator-confirmed problem wherever it lives |
| Padding a one-approach problem into fake options | Require problem-linked evidence; if there is one path, skip `decide` |
| Copying a competitor's solution as the answer | Add it as one unjudged option; ranking/choosing is `decide`'s, don't collapse generation into selection |
| Fan-out agents return ranked / evaluated options | Prompt them to generate raw only; ranking is `decide`'s |
| Starting from the parked solutions | They're seeds, one unjudged option each; starting there smuggles the old assumption back |
| Generating while the problem definition is uncertain | Reset to `define`; hold the pool |
| Absorbing the agents' output straight into the file | Show it to the operator and widen together; don't make them read the doc to see it |
| Dumping the whole pool at once | Show it a batch at a time so the operator can "yes, and" each |
| Declaring the widen closed yourself | The operator says when the pool is wide enough |
| Inferring "wide enough" from an ambiguous "yes" | Get an explicit stop; if unclear, ask, don't put words in their mouth |
| Leaving the full pool only in an optional file | Point to the file (or walk the operator through it) |
| Two questions in one turn ("batch 3, or wide enough?") | Ask one; a bundled question gets the first answered and the second misread |
| Laundering the operator's pre-decided solution | Park it as one option; push past it to get new ideas flowing |
| Treating the delivery vehicle as the solution | "An app" / SMS / web is packaging; ask what it would *do*, generate on mechanisms |
| Taking a prior prototype as "their solution" | Ask what they *learned* from it; capture the learnings as knowledge |
| Letting a PoC silently become the product | It's a seed + learnings; the real thing is built via plan → implement, not by promoting the PoC |
