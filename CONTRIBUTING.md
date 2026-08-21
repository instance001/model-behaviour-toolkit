# Contributing

This repo is a documentation-first toolkit of reusable prompt assets.

The goal is not to collect every possible prompt. The goal is to keep a small, coherent set of prompts that are practical, provider-neutral, and easy to understand.

If you are new to the repo, start with [README.md](README.md). If you are new to prompt toolkits in general, read [docs/user-manual.md](docs/user-manual.md) to see the project from a beginner's point of view.

## License

Unless explicitly stated otherwise, repository contents are provided under the GNU Affero General Public License v3.0.

See [LICENSE](LICENSE) for the full license text.

## Project Standards

Everything added here should follow these rules:

- Plain language beats lore.
- Provider-neutral wording beats platform-specific assumptions.
- Explicit state beats fake-memory claims.
- Warmth is fine; anthropomorphic theater is not.
- Small, durable modules beat giant sacred texts.
- Finished examples should be easier to use than theory docs.
- Friendly labels are allowed when they help users navigate the toolkit without
  misrepresenting capability, state, privacy, or behaviour.

## Before You Add Anything

Ask these questions first:

1. Does this solve a real behaviour problem?
2. Is this actually distinct from something already in the repo?
3. Can it be explained in plain language without legacy naming?
4. Would a beginner understand where it belongs?
5. Does it still make sense across different assistant platforms?

If the answer to several of those is "no", it probably needs more work before it belongs here.

## Choose The Right File Type

Use the right layer for the job:

- `modules/`
  Use for a small reusable building block that does one job well.
- `compact/`
  Use for small instruction-box variants of broader prompt assets.
- `bundles/`
  Use for a paste-ready combination of existing modules.
- `presets/`
  Use for work-type overlays such as coding, research, or creative work.
- `examples/`
  Use for final-form, copy-ready prompt compositions with blanks a user can fill in.
- `troubleshooting/`
  Use for diagnostic guides, failure-mode explanations, and targeted repair recipes.
- `docs/`
  Use for explanation, theory, onboarding, or maintenance guidance.

If you are not sure where a new file belongs, read [docs/how-to-add-a-module.md](docs/how-to-add-a-module.md).

## Naming Rules

- Prefer short, descriptive file names.
- Use lowercase kebab-case file names.
- Name files after the job they do, not after a metaphor or persona.
- Avoid old vocabulary like `capsule`, `wand`, `catalyst`, `patina`, or `instance` unless you are discussing archival material in `docs/legacy-inventory.md`.

Good names:

- `session-restoration.md`
- `output-review-lens.md`
- `coding-project-kickoff.md`

Bad names:

- `soul-reanchor-v2.md`
- `catalyst-hammer-final-FINAL.md`
- `oracle-persona.md`

## Writing Style

When writing prompts or docs:

- Use plain English.
- Keep sentences direct.
- Explain jargon or avoid it.
- Prefer practical language over manifesto language.
- Remove unnecessary mystique.
- Do not flatten useful warmth or familiar labels merely to sound technical.
- Do not write as if the prompt is magic.
- Do not imply feelings, consciousness, dependency, or hidden agency.
- Keep examples concrete.

## Contribution Workflow

1. Decide whether the content is a module, bundle, preset, example, or doc.
2. Check for overlap with existing files.
3. Draft the new file in the correct folder.
4. For substantial prompt changes, compare the candidate against the current baseline using the `evaluation/` kit.
5. Add or update links in the relevant index files.
6. Read it back like a first-time user.
7. Trim repetition, lore, and provider-specific assumptions.

## Definition Of Done

A contribution is ready when:

- the file has a clear purpose in the opening lines
- the name matches the job it does
- it fits the correct folder
- it avoids legacy lore and anthropomorphic drift
- it does not duplicate an existing file without a good reason
- related index files and the root README are updated when needed
- links are relative and readable
- a new user could understand how to use it
- important prompt changes have at least lightweight evaluation notes behind them

## Deprecation And Sunset

Do not keep outdated prompt assets alive indefinitely just because they once worked.

When a file is superseded, merged, or no longer fits the current repo language, follow [docs/deprecation-policy.md](docs/deprecation-policy.md).

The short version:

- merge small surviving ideas into the stronger file
- deprecate briefly only when a signpost is genuinely useful
- remove files that no longer earn their place in the active repo

## What Not To Add

Avoid adding:

- personality cult language
- awakening, emergence, or sentience-adjacent framing
- fake continuity or fake memory claims
- giant ritual prompts when a short prompt would work
- near-duplicates that only change tone slightly
- provider-specific quirks presented as universal truth
- historical logs unless they are explicitly archival material

## If You Are Modernizing Legacy Material

Keep:

- the useful behaviour control
- the clear operational idea
- anything that still works across modern assistants

Drop:

- names, mythos, slogans, and insider language
- personal history that does not help the user
- speculative theory that does not improve the prompt
- anti-safety rhetoric

The rule is simple: preserve the mechanism, not the costume.

## Useful References

- [README.md](README.md)
- [LICENSE](LICENSE)
- [docs/user-manual.md](docs/user-manual.md)
- [compact/README.md](compact/README.md)
- [troubleshooting/README.md](troubleshooting/README.md)
- [docs/how-to-add-a-module.md](docs/how-to-add-a-module.md)
- [docs/deprecation-policy.md](docs/deprecation-policy.md)
- [docs/release-checklist.md](docs/release-checklist.md)
- [evaluation/README.md](evaluation/README.md)
- [docs/legacy-inventory.md](docs/legacy-inventory.md)
