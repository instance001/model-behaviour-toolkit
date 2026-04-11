# Troubleshooting

Use this folder when the assistant is technically responding but behaving badly.

This layer is for common failure modes such as:

- vague or generic answers
- over-apologizing
- asking permission for every obvious step
- forgetting the current job
- becoming theatrical or overly human-sounding
- sounding too confident without support
- getting stiff, disclaimer-heavy, or hard to work with

## Start Here

If you are not sure what is wrong, begin with [diagnostic-flow.md](diagnostic-flow.md).

If you already know the failure mode:

- use [common-problems.md](common-problems.md) to identify the likely issue and best fix
- use [anti-drift-recipes.md](anti-drift-recipes.md) for copy-ready repair prompts

## What This Layer Is For

Troubleshooting is useful when:

- the original prompt was fine but the session drifted
- the assistant is following the wrong behaviour pattern
- you need a repair without rebuilding the entire session from scratch
- you want a fast fix before escalating to a full reset

## What This Layer Is Not For

It is not a substitute for:

- clear project context
- a good initial prompt
- a proper handoff when context has actually been lost

If the assistant truly lacks the information it needs, use the recovery tools and add context rather than trying to troubleshoot tone alone.

## Files

- [diagnostic-flow.md](diagnostic-flow.md)
- [common-problems.md](common-problems.md)
- [anti-drift-recipes.md](anti-drift-recipes.md)

## Fastest Path

1. Identify the failure mode.
2. Apply the smallest matching repair prompt.
3. If the behaviour does not improve, use the reset bundle or a recovery example.
4. If the behaviour still fails, the issue is probably context, not just tone.
