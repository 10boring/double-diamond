---
name: discover
description: Use when starting a design decision and the PROBLEM isn't yet grounded in reality, the Double Diamond's first move (Discover, the problem-space widen). Runs BEFORE `define`. Also called (industry synonyms): explore, research, empathize, investigate, scope, immerse, understand the problem. Trigger on "discover", "explore the problem", "research the problem", "empathize", "understand the users", "what's really going on", "ground this", Swedish "utforska problemet", "gräv i det", "vad är det egentliga problemet". Widens on the problem from real-world/user reality and produces raw problem material; it does not write a problem statement (that is `define`) and proposes no solutions.
---

# discover

The **first move** of the Double Diamond (design thinking): **Discover**, the problem-space
**widen**. It runs before `define` (which narrows the discovery to one problem statement). The
method's first rule: understand the problem before you solve it, and the first diamond is about
the **problem**, never the solution.

## Core principle

Understand, don't assume, what the problem is. `discover` widens on the problem from **independent
sources** and, above all, **real-world reality**: what actually happens, who the users are, what
exists today. It proposes **no solutions**; if one surfaces, park it. The whole pipeline's rigor
starts here, a solution built on an unexamined problem is wasted work.

## When to skip it

If the problem is already grounded and agreed (you can state what's wrong in one sentence and it
rests on observed reality, not assumption), go straight to `define`. Don't manufacture discovery
for a settled problem.

## Working file

Create the effort's working file **in the repo you're working in**, under
`docs/designthinking/<slug>.md`, so the operator can read and version it alongside the code. Only
if you are not in a repo, fall back to `~/.claude/design/<slug>.md`. (`<slug>` derived from the
problem.) This skill creates it with this skeleton and fills `## Discover`, leaving the later
sections for the downstream skills:

```markdown
# Design: <slug>
Status: discovering | defining | developing | deciding | probing | ready-to-specify

## Discover   (discover)  current reality + raw problem material, UNJUDGED
## Define     (define)    reframed problem statement + surfaced assumptions
## Develop    (develop)   raw option pool, UNJUDGED
## Decide     (decide)    criteria + the one chosen idea
## Probe      (probe)     riskiest assumption + test card + verdict
→ Handoff: brainstorming to specify "<chosen idea>", then plan → implement → MVP/MVF
```

`Status` is the precondition gate for every phase; set it to `defining` once `## Discover` is
written. Phases re-enter freely and `Status` moves both ways; the working file is a **living
document**, revised in place, not only appended.

## Workflow

1. **Widen on the PROBLEM from reality (judgment deferred, no solutions).** Operator first so you
   don't anchor:
   - **Operator first, one question at a time.** Discover is a conversation, not a questionnaire:
     ask **one focused question per turn**, wait, then follow up. Start with what is actually
     wrong / what triggered this, and invite the messy version.
   - **Real users, not just the operator.** Design thinking's first stage is *empathy*, the
     problem belongs to real users, so ground it in **their** reality (talk to one, observe, read
     real usage), not only the operator's account or your own. When the operator is **not** a
     user, say so and treat a real user as the primary source.
   - **Current reality first, for a redesign.** When reframing an *existing* system, **inventory /
     audit** what's actually there (what exists, who owns each part, how it flows) before
     problem-lens brainstorming.
   - **Parallel agents.** Fan out 3–4 subagents on distinct *problem* lenses (what is really being
     solved / root and adjacent problems / how others frame this / the assumption baked into the
     ask), blind to each other; pool and dedup. **Agent agreement is breadth, not evidence**, a
     unanimous panel can be confidently wrong; a single operator/user fact outranks it.
   - Do **not** converge or propose solutions here (that is `define` and `develop`).
2. **Write and hand off.** Write the `## Discover` section (current reality + raw problem material,
   unjudged), set `Status: defining`, and point to `define`.

## What it does NOT do

- **No problem statement** — that is `define`. Discover gathers; Define distills.
- **No solutions** — park any that surface.
- **Doesn't ground from one mind** — real users + operator + agents, never introspection alone.

## Common mistakes

| Mistake | Right |
|---------|-------|
| Jumping to a problem statement | That is `define`; gather first |
| Framing from a non-user's introspection | Ground in real users; the operator may not be one |
| Treating agent consensus as evidence | Breadth, not proof; user/operator facts outrank it |
| Jumping to solutions | Park them; discover is problem-only |
| Discovering a problem that is already grounded | Skip to `define` |
