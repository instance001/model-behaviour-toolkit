# Changelog

All notable changes to this repo should be recorded here.

This changelog tracks the modernized `model-behaviour-toolkit` repo, not the full historical contents of the legacy archive folders it was built from.

## [Unreleased]

### Added

- A new `evaluation/` layer with a run protocol, scoring rubric, benchmark tasks, and scorecard template
- A new `compact/` layer with tiny and short variants for general, reset, coding, research, and creative use
- A new `troubleshooting/` layer with a diagnostic flow, common failure modes, and anti-drift repair prompts
- A deprecation policy for merging, signposting, and removing outdated prompt assets as the toolkit evolves

### Changed

- Root onboarding now points users with cramped instruction boxes toward `compact/`
- Root onboarding and beginner docs now point users toward troubleshooting when the assistant drifts or misbehaves
- Contributor and release guidance now includes the evaluation layer, compact variants, troubleshooting paths, and deprecation rules
- Merged the standalone restoration template into `modules/recovery/session-restoration.md`
- Folded compact platform guidance into `compact/README.md`
- Deprecated `examples/session-recovery-with-handoff.md` as a temporary signpost in favor of `bundles/reset-bundle.md` plus `modules/operator/session-handoff.md`

### Planned

- Additional examples and presets as real gaps appear
- Further trimming or archival separation of legacy source material in the wider workspace
- Future release notes as the toolkit evolves

## [0.1.0] - 2026-04-11

### Added

- Root repo scaffold and core positioning in [README.md](README.md)
- Legacy migration audit in [docs/legacy-inventory.md](docs/legacy-inventory.md)
- Beginner onboarding in [docs/user-manual.md](docs/user-manual.md)
- Maintainer guidance in [CONTRIBUTING.md](CONTRIBUTING.md)
- Module authoring guide in [docs/how-to-add-a-module.md](docs/how-to-add-a-module.md)
- Release hygiene guide in [docs/release-checklist.md](docs/release-checklist.md)

### Added: Core Modules

- Baseline modules for session setup and boundary-aware collaboration
- Recovery modules for restoration, portable reset, and restoration templates
- Operator modules for handoff and execution contracts
- Review and exploration modules for output checking and creative reframing

### Added: Higher-Level Composition Layers

- Paste-ready bundles in `bundles/`
- Work-type presets in `presets/`
- Copy-ready example workflows in `examples/`

### Changed

- Reframed the project around plain-language, provider-neutral prompt assets
- Replaced lore-heavy, persona-heavy, and era-specific framing with practical module names and clear usage guidance
- Established a clearer separation between beginner docs, contributor docs, and archival analysis

### Notes

- This is the first clean release of the rebuilt repo structure
- Legacy archive folders remain outside this repo and are treated as source material, not release history
- The modernized repo is released under the GNU Affero General Public License v3.0; see [LICENSE](LICENSE)
