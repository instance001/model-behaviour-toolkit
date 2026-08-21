# How To Add A Module

This guide is for contributors who want to add a new file to the toolkit without making the repo messier.

It assumes you understand the basic purpose of the repo but want a concrete workflow.

## First Question: Does This Need To Be A Module?

A module should be:

- small
- reusable
- focused on one job
- useful across more than one workflow

Good module candidates:

- a session reset prompt
- a handoff template
- a review lens
- a mode switch for a specific kind of behaviour

Bad module candidates:

- a giant all-in-one prompt that tries to do everything
- a compact variant that belongs in `compact/`
- a domain-specific workflow that belongs in `presets/`
- a finished copy-ready composition that belongs in `examples/`
- a diagnostic or repair guide that belongs in `troubleshooting/`
- a combination of existing modules that belongs in `bundles/`

## Decide Where It Belongs

Use this quick test:

- Put it in `modules/` if it is a building block.
- Put it in `compact/` if it is a small instruction-box variant.
- Put it in `bundles/` if it combines multiple modules into a general default.
- Put it in `presets/` if it tunes behaviour for a type of work.
- Put it in `examples/` if it is a finished prompt someone can copy and fill in.
- Put it in `troubleshooting/` if it diagnoses failure modes or gives repair paths.
- Put it in `docs/` if it explains the repo or the reasoning behind it.

## Choose A Folder Inside `modules/`

Current module groups:

- `modules/baseline/`
  Default working mode and tone anchors.
- `modules/recovery/`
  Reset, restoration, and continuity-repair prompts.
- `modules/operator/`
  Execution rules, handoffs, and workflow coordination.
- `modules/review/`
  Evaluation and self-check prompts.
- `modules/exploration/`
  Creative or speculative mode switches.

If a new module does not fit any of those, that does not automatically mean we need a new folder. Often it means the module needs to be simplified or folded into an existing area.

## Name The File

Use lowercase kebab-case.

Name the file after what it does.

Good:

- `decision-audit.md`
- `meeting-summary-handoff.md`
- `source-quality-check.md`

Bad:

- `phoenix-seed.md`
- `cognitive-rebind-engine.md`
- `ultimate-master-mode.md`

## Module Structure

Most modules in this repo follow a simple structure:

1. Title
2. One-sentence or two-sentence use case
3. Short explanation of what the module does
4. Copy-ready prompt block
5. Optional notes such as best use cases, add-ons, or warnings

## Copy Template

Use this as a starting point:

````md
# Module Name

Use this when [plain-language use case].

This module helps with [one clear problem].

## What It Does

- [behaviour effect]
- [behaviour effect]
- [behaviour effect]

## Prompt

```text
[copy-ready prompt goes here]
```

## Best Use Cases

- [use case]
- [use case]

## Notes

- [optional limitation, pairing note, or warning]
````

If the module is simple enough, you do not need every section. Do not bulk it up just to match a pattern.

## Writing Rules

When drafting the prompt itself:

- use plain language
- avoid platform-specific assumptions unless clearly labeled
- avoid claims of hidden memory
- avoid personality or awakening language
- keep warmth practical
- preserve friendly labels when they help the user and do not mislead about
  capability, state, privacy, or behaviour
- make the intended behaviour explicit
- prefer short instruction lists over sprawling paragraphs

## Modernization Test

If the module came from legacy material, apply this test:

1. Remove legacy names and mythology.
2. Remove personal backstory.
3. Remove any claim that the assistant is secretly more alive or aware than it is.
4. Remove any line that only made sense for an older platform limitation.
5. Check whether the useful prompt still survives.

If the useful part disappears when you remove the lore, the original probably was not strong enough to keep.

## Check For Overlap

Before adding a new module, compare it against nearby files.

Common repo failure modes:

- two modules that do almost the same thing
- one module that should really be an add-on inside another file
- a new file created because the wording changed, not because the function changed

If the new file only differs in style, consider adding a short variant or note to an existing module instead.

## After Adding The File

Update the relevant surfaces:

- the local folder README, if there is one
- the root [README.md](../README.md) if the new file changes onboarding or core repo structure
- any bundle, preset, or example that should point to the new module

## Review Checklist

Before you consider the module done, check:

- Does the opening line clearly say when to use it?
- Is the file name plain and descriptive?
- Is the prompt copy-ready?
- Would a beginner understand what problem it solves?
- Does it avoid lore, fake memory, and anthropomorphic drift?
- Does it belong in `modules/` rather than another folder?
- Did you update the relevant links?

## Example Decision

Suppose you want to add a prompt that helps the assistant double-check whether a recommendation is based on outdated information.

That likely belongs in:

- `modules/review/` if it is a reusable checking prompt
- `compact/` if it is only a short instruction-box version of an existing check
- `presets/research.md` if it is just a research-specific addition
- `examples/` if it is a full composed workflow with framing and blanks to fill in

That is the main pattern for this repo:

Start small.

Only move upward into bundles, presets, or examples when the composition itself is useful.
