# Double Diamond operating contract

Read this before running any Double Diamond skill.

## Mandate and boundary

Double Diamond owns whether and what to build. Superpowers owns specification, planning, TDD,
implementation, review, and delivery. Ceremony scales with uncertainty, consequence, and
reversibility; responsibility for answering "is this the right thing to build?" does not.

## Evidence gates

Gate on sufficient evidence for the question in front of you, never on completed phases, headings,
files, or `Status`. The operator owns product choices; the agent owns the reasoning structure.
Operator confirmation is required when the product decision changes. Agent consensus supplies
breadth, never real-world evidence. A surprising answer or contradiction is a firm stop: deepen,
probe, or reset. Moving backward is normal iteration.

## Proportional techniques

Use one strong pass by default. Use multi-agent fan-out when stakes are high, the search space is
broad, or a first pass reveals real uncertainty. Use workshops and voting only for a genuinely wide
field or multiple stakeholders. Preserve real-user grounding, the non-user guard, generation kept
separate from evaluation, and thresholds fixed before probe results are seen.

## Probe anywhere

`probe` is a cross-cutting learning tool, not a mandatory station. Invoke it from any phase when a
material uncertainty could change the decision. Return its evidence to the phase whose question it
tested. Interviews, observations, research, measurements, spikes, prototypes, PoCs, and real-product
experiments may all be probes.

## Artifact and handoff

A working file is optional during reasoning. At completion, write a proportional handoff to
`docs/designthinking/<slug>.md` with four minimum headings: `Problem`, `Solution`, `MVP/MVF`, and
`Verdict`. Add evidence, alternatives, requirements, acceptance criteria, exclusions, uncertainty,
and learning criteria only when material.

The handoff must trace: defined user problem -> solution mechanism -> MVP/MVF -> expected user
outcome. The `MVP/MVF` section must name the minimal real product or feature experiment used by real
customers and a measurable product-level signal that shows whether it solves the defined problem.
The `Verdict` section must record the evidence-backed right-thing conclusion and the operator's
explicit confirmation. Superpowers may refine detailed behavior, but a material change to the
problem, chosen solution, MVP/MVF boundary, or product-level success signal returns to Double
Diamond.
