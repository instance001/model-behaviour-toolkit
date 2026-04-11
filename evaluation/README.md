# Evaluation

This folder exists to answer a simple question:

Did a new prompt asset actually improve anything?

Without an evaluation layer, a prompt repo can turn into a cleaner-looking version of the same old pile: more files, more confidence, not much proof.

## What This Is For

Use the evaluation kit when you are:

- adding a new module, bundle, preset, or example
- revising an existing prompt asset
- comparing two variants of the same idea
- deciding whether a prompt should be kept, merged, or dropped
- preparing a release

## What Is In This Folder

- [rubric.md](rubric.md)
  The scoring rubric for judging outputs.
- [benchmark-tasks.md](benchmark-tasks.md)
  A starter set of test tasks for coding, research, creative work, and recovery.
- [scorecard-template.md](scorecard-template.md)
  A copy-ready template for recording results.
- [run-protocol.md](run-protocol.md)
  The procedure for running a fair comparison.

## Basic Workflow

1. Pick the asset you want to evaluate.
2. Pick the benchmark tasks that match its intended use.
3. Run the same task with the same model and conditions.
4. Score the output with [rubric.md](rubric.md).
5. Record the result in [scorecard-template.md](scorecard-template.md).
6. Compare the results against the current baseline.

## Important Rules

- Change one variable at a time.
- Keep the model, settings, and task wording the same when comparing variants.
- Save the raw outputs if the comparison matters.
- Do not rely only on "this feels better".
- Use both scores and short notes.

## What Good Evaluation Looks Like

Good evaluation is:

- small
- repeatable
- relevant to the prompt's real job
- harsh enough to catch regressions

It does not need to be elaborate to be useful.

## Start Here

If you only want the shortest path:

1. Read [run-protocol.md](run-protocol.md).
2. Use one task from [benchmark-tasks.md](benchmark-tasks.md).
3. Score it with [rubric.md](rubric.md).
4. Record the result in [scorecard-template.md](scorecard-template.md).
