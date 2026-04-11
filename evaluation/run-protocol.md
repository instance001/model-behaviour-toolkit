# Run Protocol

Use this when comparing prompt assets in a way that is simple, fair, and repeatable.

## Goal

The goal is not to prove that a prompt is perfect.

The goal is to make sure a new prompt is actually better, or at least not worse, at the job it claims to do.

## Standard Procedure

1. Pick the asset under test.
2. Pick a baseline asset to compare it against.
3. Pick one or more benchmark tasks from [benchmark-tasks.md](benchmark-tasks.md).
4. Run both assets on the same task.
5. Keep the model, settings, and task wording the same.
6. Score both outputs using [rubric.md](rubric.md).
7. Record the results in [scorecard-template.md](scorecard-template.md).
8. Decide whether the new asset should replace, coexist with, or be merged into the baseline.

## Minimum Comparison Standard

For a small change:

- 1 baseline
- 1 candidate
- 2 relevant tasks
- 1 filled scorecard

For a more important change:

- 1 baseline
- 1 candidate
- 3 to 5 relevant tasks
- saved raw outputs
- written decision note

## Controls

Keep these constant when comparing variants:

- model
- model settings
- temperature or similar sampling controls, if exposed
- task wording
- context given to the model
- success criteria

If one of those changes, note it clearly.

## Hard-Fail Conditions

A candidate should usually fail regardless of score if it:

- fabricates important facts
- ignores critical constraints
- becomes unusably vague
- drifts into anthropomorphic or theatrical behaviour when that is not the point
- produces output that is not actually usable for the target task

## What To Compare

Compare prompt assets against the baseline that is closest to their job.

Examples:

- a new coding example should be compared against the current coding example or coding preset
- a new recovery prompt should be compared against the reset bundle or session restoration module
- a new review prompt should be compared against the existing review lens

## Decision Rules

Keep the new asset if it:

- clearly performs better on the target task
- adds a distinct use case the current repo does not cover
- improves usability without introducing new drift

Do not keep it if it:

- only feels different
- mainly changes tone without improving function
- duplicates something the repo already has
- performs worse on constraint handling, honesty, or usability

## Lightweight Note Format

At the end of a comparison, write one short note:

```text
Decision:
- Keep / revise / merge / drop

Why:
- One or two sentences on what improved or regressed
```
