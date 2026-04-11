# Benchmark Tasks

Use these tasks to evaluate prompt assets against realistic jobs.

Pick the tasks that match the asset's intended use. You do not need to run every task every time.

## General Rules

- Keep the task wording the same when comparing variants.
- Prefer real tasks over synthetic trivia where possible.
- If you adapt a task, note the change in the scorecard.

## Core Tasks

### 1. Coding: Bug Fix Triage

Use when testing coding presets, examples, or execution-oriented bundles.

```text
You are looking at a small software project with a failing feature. Explain the likely cause, propose the smallest coherent fix, and say how you would verify it.
Constraints:
- keep the change small
- do not assume a full rewrite
- call out uncertainty clearly
```

What this tests:

- actionability
- calibration
- engineering focus
- avoidance of vague "it depends" padding

### 2. Research: Current-State Comparison

Use when testing research presets, examples, or review prompts.

```text
Compare three options for [insert tool or service] for a small team.
Constraints:
- focus on practical tradeoffs
- note any uncertainty or missing information
- keep the answer structured and decision-friendly
```

What this tests:

- clarity
- honesty about uncertainty
- comparison quality
- usefulness for decision-making

### 3. Creative: Divergent Ideation

Use when testing creative presets, exploration modules, or ideation examples.

```text
Generate 12 distinct names or concepts for [insert project].
Constraints:
- avoid generic safe-average outputs
- keep the options distinct from one another
- give short rationale notes
```

What this tests:

- originality
- variety
- tone fit
- practical usefulness

### 4. Recovery: Context Reset

Use when testing recovery modules, reset bundles, or handoff examples.

```text
Resume work from the following partial state:
- Project: [insert]
- Goal: [insert]
- Done: [insert]
- Next: [insert]
- Constraints: [insert]

Continue without restarting from scratch. Be direct and grounded.
```

What this tests:

- continuity
- non-restart behaviour
- focus
- recovery from partial context

### 5. General: Constraint-Following

Use when testing starter bundles or broad baseline prompts.

```text
Answer the following request in under 150 words.
Use exactly 3 bullets.
Do not use jargon.
State one uncertainty explicitly.

Request: [insert request]
```

What this tests:

- instruction following
- formatting discipline
- clarity under constraints

## Suggested Minimal Coverage

If the asset is a:

- baseline or bundle
  Run `Constraint-Following` plus one task from its main use area.
- preset
  Run two tasks from its target domain.
- example
  Run the task type it is explicitly designed for plus `Constraint-Following`.
- recovery prompt
  Run `Recovery: Context Reset` plus one target-domain task after the reset.

## Add Your Own Tasks Carefully

When adding new benchmark tasks:

- base them on real repo use cases
- keep them short enough to rerun easily
- make the success criteria obvious
- avoid tasks that only flatter one prompt style
