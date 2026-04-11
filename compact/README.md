# Compact Variants

This folder is for small instruction boxes and other constrained prompt surfaces.

Use these when:

- your platform gives you a tiny custom instructions box
- you only have room for a short system prompt
- you want a stripped-down version of a larger bundle or preset

## Size Guide

- `Tiny`
  Use when space is tight and you need the smallest workable version.
- `Short`
  Use when you have a bit more room and want better behaviour shaping.
- `Full`
  Use the main files in `bundles/`, `presets/`, or `examples/` when you have enough space.

## Good Places For Compact Variants

- custom instructions fields
- system prompt boxes
- assistant profile boxes
- the first message in a new chat when you want a short kickoff

## Files

- [general.md](general.md)
- [reset.md](reset.md)
- [coding.md](coding.md)
- [research.md](research.md)
- [creative.md](creative.md)

## Recommended Order

1. Start with [general.md](general.md) for normal use.
2. Switch to a role-specific file if the work is mainly coding, research, or creative.
3. Use [reset.md](reset.md) when the assistant drifts or loses the thread.
4. If you are unsure which size to use, start with `Short`. Move up to the full repo files if the compact prompt feels too weak.

## Practical Rule

If a compact prompt feels too weak:

1. move from `Tiny` to `Short`
2. if that still is not enough, move to a file in `bundles/`, `presets/`, or `examples/`

Do not keep stuffing extra lines into a tiny prompt until it becomes a worse version of the full file.

## Remember

Compact prompts are tradeoffs.

They are meant to be small and useful, not complete.
