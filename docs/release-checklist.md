# Release Checklist

Use this before calling the repo ready for a versioned release, public share, or wider handoff.

The point of this checklist is not ceremony. It is to keep the repo coherent as it grows.

## 1. Repo Shape

- The root [README.md](../README.md) still reflects the real repo structure.
- New folders or file types are linked from the right index files.
- There are no orphaned files that a new user would never discover.
- Beginner, contributor, and example paths still make sense.

## 2. Onboarding

- [docs/user-manual.md](user-manual.md) still matches the current repo layout.
- [examples/README.md](../examples/README.md) is still the easiest entry point for beginners.
- [bundles/README.md](../bundles/README.md) and [presets/README.md](../presets/README.md) still point users in the right direction.
- Troubleshooting paths still make sense when the assistant drifts or misbehaves.
- The quickest path for a first-time user is still obvious.

## 3. Content Quality

- New prompts solve a real problem and are not just stylistic variants.
- Important new prompt assets have been checked against the current baseline using the `evaluation/` kit.
- Superseded files have been merged, deprecated clearly, or removed instead of lingering ambiguously.
- There is no unnecessary lore, mythology, or insider language.
- File names are plain, descriptive, and kebab-case.
- Prompts are provider-neutral unless clearly labeled otherwise.
- Prompts do not imply feelings, consciousness, fake memory, or hidden agency.
- Giant ritual prompts have not crept back in where a shorter one would do.

## 4. Structural Hygiene

- Modules, compact variants, bundles, presets, examples, troubleshooting guides, evaluation assets, and docs are each being used for the right job.
- Similar files have been merged or differentiated clearly.
- Index files and cross-links use readable relative paths.
- Copy-ready prompts still render cleanly in Markdown.

## 5. Beginner Experience

- A new user can start with one file and succeed without reading the whole repo.
- Example files still include the right blanks to fill in.
- Jargon is explained or removed.
- The repo does not assume prior prompt-engineering knowledge.

## 6. Contributor Experience

- [CONTRIBUTING.md](../CONTRIBUTING.md) still matches how the repo is actually maintained.
- [docs/how-to-add-a-module.md](how-to-add-a-module.md) still reflects the current folder structure.
- The authoring rules still discourage duplication and lore creep.

## 7. Legacy Boundaries

- Historical material remains clearly separated from modern toolkit content.
- Archive references stay inside explanatory docs unless there is a strong reason otherwise.
- Legacy naming is not leaking back into active files except where archival context requires it.
- Recently replaced files follow the deprecation policy instead of piling up beside their replacements.

## 8. Pre-Release Sweep

- Read the root README as if you have never seen the repo before.
- Read the beginner manual as if you know nothing about prompt toolkits.
- Read the contributor guide as if you are about to add a new file.
- Spot-check the evaluation layer and confirm it still matches current repo structure.
- Spot-check the troubleshooting layer and confirm the repair paths still point to the right files.
- Spot-check at least one bundle, one preset, and one example.
- Search for obvious regressions such as `TODO`, `placeholder`, or accidental archive jargon in active files.

## 9. Release Notes

Before tagging or sharing a release, write a short note covering:

- what changed
- what was added
- what was removed or deprecated
- whether the beginner path changed
- whether contributor guidance changed

## Minimal Release Standard

If you are in a hurry, at minimum confirm:

1. The root [README.md](../README.md) is accurate.
2. The beginner path still works.
3. The contributor path still works.
4. New files are linked and categorized correctly.
5. No obvious lore, duplication, or broken onboarding slipped back in.
