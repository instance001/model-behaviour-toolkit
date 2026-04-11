# Deprecation Policy

This repo is meant to evolve with changing models, tools, and prompt practices.

That means some prompt assets will age out.

This policy exists to stop the repo from turning back into a pile of half-obsolete tools with slightly different names.

## Core Rule

When a prompt asset no longer earns its place, do one of three things:

- merge it
- deprecate it briefly with a clear replacement
- remove it

Do not leave it hanging around as a vague maybe-still-useful relic.

## Goals

The deprecation policy is here to keep the repo:

- small
- current
- easy to navigate
- free of duplicate generations of the same idea

This matters because prompt tools age quickly. New model behaviour, longer context, better tooling, and different product surfaces can make older prompt patterns unnecessary or actively worse.

## Deprecation States

Use these states when evaluating an existing file.

### 1. Active

The file is current, useful, and should stay in normal repo navigation.

### 2. Merge

The file still contains useful material, but not enough to justify standing alone.

Action:

- fold the surviving content into the better file
- remove the redundant file
- note the change in the changelog if it matters

### 3. Deprecated

The file is no longer recommended, but it needs a short transition period because:

- people may still be linking to it
- the replacement is new enough that a signpost helps
- removing it immediately would create confusion

Action:

- keep the file temporarily
- add a clear note at the top pointing to the replacement
- remove it from primary onboarding surfaces
- plan removal in a future release

### 4. Removed

The file no longer belongs in the active repo.

Action:

- delete it from the active structure
- rely on git history and release notes for historical traceability

## When To Deprecate A File

Deprecate or remove a file if one or more of these are true:

- it duplicates another asset with only small wording changes
- it reflects outdated platform assumptions
- it uses naming or framing the repo is actively moving away from
- it has been replaced by a clearer bundle, preset, example, or compact variant
- evaluation shows it performs worse than the current baseline
- it confuses users more than it helps them

## When To Merge Instead Of Deprecate

Merge when:

- the file has one or two useful lines but not a full distinct use case
- the difference is mostly tone, not function
- the existing replacement already covers the same job

The repo should prefer fewer stronger files over a family of near-duplicates.

## How To Mark A Deprecated File

If a file must stay temporarily, add a short note at the top like this:

```md
> Deprecated: use [replacement-file.md](replacement-file.md) instead.
> This file is being kept briefly as a signpost and may be removed in a future release.
```

Keep it short.

Do not write a long apology or historical essay inside the file.

## Where Deprecated Files Should Appear

Deprecated files should:

- stay out of the main beginner path
- stay out of the primary quick-start path
- stay out of the main bundle/preset/example indexes when possible

If they must remain visible for transition reasons, they should be clearly labeled.

## Preferred Replacement Strategy

When replacing an old file:

1. identify the best surviving function
2. rewrite it in current terminology
3. point the old file to the new one if a short transition period is needed
4. remove the old file once the signpost period is no longer useful

This is exactly the pattern behind retiring terms like `wand`, `capsule`, and similar older framing.

## Decision Questions

Before keeping an older file around, ask:

1. Does this still outperform or materially differ from the replacement?
2. Is it teaching users the current repo language or dragging them back into old terminology?
3. Would a new user be better off if this file simply did not exist?

If the answer to the third question is yes, remove it.

## Release Expectations

Before a release:

- review recently replaced files
- remove any deprecated files that no longer need a transition period
- make sure replacements are linked clearly
- note removals or deprecations in the changelog when they affect navigation

## What Not To Do

Avoid these habits:

- keeping every old version "just in case"
- renaming a file but keeping the old one beside it forever
- adding version suffixes to avoid making a decision
- treating git history as something separate from the repo's archival function

Git history already preserves history.

The active repo should preserve usability.
