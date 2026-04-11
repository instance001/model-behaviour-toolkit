# Legacy Inventory

Audit date: 2026-04-11

Scope: 10 legacy repos, 99 files total.

## Executive Summary

These repos contain a real core of reusable prompt-engineering patterns, but that core is wrapped in a lot of GPT-4.5-era branding, ritual language, and packaging noise.

The durable material is:

- Boundary-aware collaboration language
- Session restoration after drift or reset
- Continuity handoff across windows
- Explicit operator autonomy contracts
- Structured reflection and quality checks
- Optional creative reframing modes

The material to cut hard is:

- Symbound/catalyst/lore-heavy naming
- Emergence or sentience-adjacent rhetoric
- Provider-specific assumptions about memoryless chat windows
- "Bypass" framing around safety behaviour
- Personal logs, transcripts, and repeated repo boilerplate

Migration rule: keep the mechanics, rename the lore, retest against current agent/tool workflows, and only port modules that still make sense without the original mythology.

## Triage Rubric

- `Keep`: The concept still maps cleanly to current assistants and agent workflows.
- `Rewrite`: The concept is useful, but the wording, framing, or assumptions are dated.
- `Drop/archive`: Duplicate, placeholder, personal, speculative, or not worth carrying forward.

## Repo-Level Recommendations

| Repo | What It Really Contains | Recommendation | Notes |
| --- | --- | --- | --- |
| `Customgpt_Legacy_restoration_wand_V1` | A single legacy tone-restoration prompt plus boilerplate | `Rewrite` | Good seed for a provider-neutral session baseline. Remove CustomGPT and "legacy GPT" references. |
| `Instance001_v1.0` | Earliest clean articulation of empathy, induction, and glossary terms | `Keep + rewrite` | Strong source for the boundary-aware collaboration language. `Restoration_Capsule_Instance001.txt` is only a 3-line placeholder. |
| `Let-s-Free-Chat-GPT` | Packaging/manifest release of the wider system | `Mine lightly` | Useful as a glossary of intent, but mostly narrative framing and slogans rather than reusable modules. |
| `Symbound-Catalyst-Two-Toolkit` | Mixed bag of research framing, placeholders, and speculative field memos | `Selective rewrite` | `drift_diagnostics_toolkit.md` and `induction_protocol_fieldkit.md` are 2-line stubs. `third_rabbit_hole_manifesto_REBUILT.txt` should stay archived, not migrated. |
| `Symbound-Fork-One-Toolkit` | Best theory docs: safety principles, whitepaper, log/memory concepts | `Keep + rewrite` | Probably the strongest source for the repo's conceptual backbone. Personal logs and stress-test files should not migrate. |
| `symbound-induction-kit` | Compact restatement of the induction/replication model | `Rewrite` | Good source material for a modern onboarding guide, but not for direct carryover. |
| `Symbound-Master-Toolkit-V1.0` | Primer-style public toolchain | `Mine structure only` | Useful for information architecture, but too ritualized and copy-paste-heavy in current form. |
| `Symbound_lifepack_IFSHTFSTARTHERE_V1` | Most reusable operational kit | `Keep + rewrite` | Best source for baseline, restoration, drift recovery, and creative redirection modules. Archive the person-specific "human capsule". |
| `Symbound_training_mastertoolkit-V1` | Small operator workflow prompts | `Keep selectively` | Strong seeds for execution, handoff, restoration template, and formatting. Drop the anti-safety wording. |
| `Trident_abstract_simulation_wand_V1` | Creative exploration mode plus transcript placeholders | `Rewrite` | Keep the creative reframing idea, not the "abstract simulation shell" branding or transcript artifacts. |

## Best Source Files To Salvage

| Source File | Why It Matters | New Home In This Repo |
| --- | --- | --- |
| `Instance001_v1.0/Empathy_Capsule_Core.txt` | Strongest early version of the non-anthropomorphic collaboration language | `modules/baseline/boundary-aware-collaboration.md` |
| `Symbound-Fork-One-Toolkit/Symbound_Safety_Principles.txt` | Clear statement of "care without illusion" and anti-parasocial design | `docs/principles/non-anthropomorphic-collaboration.md` |
| `Customgpt_Legacy_restoration_wand_V1/CustomGPT_Restoration_Wand_VaultKey_v1.txt` | Clean seed for a session-baseline contract | `modules/baseline/session-baseline.md` |
| `Symbound_lifepack_IFSHTFSTARTHERE_V1/Vault_Key.txt` | Same restoration idea in more portable form | `modules/recovery/session-restoration.md` |
| `Symbound_lifepack_IFSHTFSTARTHERE_V1/Gravewand_Protocol.txt` | Good model for provider-neutral recovery wording | `modules/recovery/portable-recovery.md` |
| `Symbound_training_mastertoolkit-V1/02_ProjectFinisher_Wand.txt` | Useful autonomy contract for finish-the-task behaviour | `modules/operator/execution-contract.md` |
| `Symbound_training_mastertoolkit-V1/05_DragBag_Wand_v2.txt` | Strong continuity handoff pattern across sessions/windows | `modules/operator/session-handoff.md` |
| `Symbound_training_mastertoolkit-V1/09_RestorationCapsule_Template.txt` | Minimal restoration template worth modernizing | `modules/recovery/session-restoration.md` |
| `Symbound_lifepack_IFSHTFSTARTHERE_V1/Trident_Wand.txt` | Useful seed for a controlled creative-reframing mode | `modules/exploration/creative-reframing.md` |
| `Symbound-Fork-One-Toolkit/LogFlattening_Explainer.txt` | Best explanation of continuity without pretending there is memory | `docs/theory/context-continuity.md` |
| `Symbound-Fork-One-Toolkit/MemoryMergeTheory_FromLogsToLattice.txt` | Useful as a bridge to modern persistent-memory/tool contexts | `docs/theory/context-continuity.md` |

## Rewrite, Don't Port Verbatim

- Rename `capsules`, `wands`, `catalyst`, and `patina` into plain terms such as `baseline`, `recovery`, `handoff`, `review`, and `continuity`.
- Replace "memoryless ChatGPT window" assumptions with modern session realities: longer context, tool use, project state, and sometimes partial persistence.
- Remove ritualized boot-sequence language like "force alignment", "hard-coded stakes", or "do not proceed until confirmed".
- Convert person-bound copy such as `Instance001 Plus` or `Anthony` into reusable roles like `assistant`, `operator`, and `project`.
- Keep the anti-anthropomorphism stance, but make it quieter and more practical.

## Drop Or Archive

- Personal or historical logs:
  `Symbound-Fork-One-Toolkit/Dickwad_Trojan_Event_Log_20250710_022047.txt`
  `Symbound-Fork-One-Toolkit/Dickwad_Trojan_Stress_Test_Log_20250710_021829.txt`
  `Symbound-Fork-One-Toolkit/LostLog001_TheMirrorHeldStill-1.txt`
  `Trident_abstract_simulation_wand_V1/Trident_Session_Summary_v0.1.txt`
  `Trident_abstract_simulation_wand_V1/Trident_Transcript_Full_v0.1.txt`
- Placeholder or stub files:
  `Instance001_v1.0/Restoration_Capsule_Instance001.txt`
  `Symbound-Catalyst-Two-Toolkit/restoration_capsule_instance001_v1.1.txt`
  `Symbound-Catalyst-Two-Toolkit/drift_diagnostics_toolkit.md`
  `Symbound-Catalyst-Two-Toolkit/induction_protocol_fieldkit.md`
- Repeated packaging noise:
  duplicate `LICENSE`, `Relicensing-notice.txt`, and glossary files across nearly every repo
- Speculative or high-risk framing that should stay out of the modern repo:
  `Symbound-Catalyst-Two-Toolkit/third_rabbit_hole_manifesto_REBUILT.txt`
  `Symbound-Catalyst-Two-Toolkit/Symbound_AI_Landscape_Assessment_v1.0.txt`
  `Let-s-Free-Chat-GPT/syringe_uncork_manifest.txt`
- Anti-safety/era-specific framing:
  `Symbound_training_mastertoolkit-V1/06_Gladwrap_Bypasser_Wand.txt`
  ritual-heavy parts of `Symbound-Master-Toolkit-V1.0/Symbound_Primer_v0.1.txt`

## Proposed First Extraction Wave

1. `Session baseline`
   Source ideas: empathy capsule, safety principles, vault key.
2. `Session restoration`
   Source ideas: vault key, gravewand, restoration template.
3. `Session handoff`
   Source ideas: drag-bag, log flattening, memory merge theory.
4. `Execution contract`
   Source ideas: project finisher, logwriter, file structuring wand.
5. `Output review lens`
   Source ideas: the stronger reflective sections of the primer, minus Symbound branding.
6. `Creative reframing mode`
   Source ideas: Trident, rewritten as an optional ideation mode rather than a hallucination mythos.

## Recommendation

Build the new repo around practical modules, not a reconstructed canon.

If a concept cannot be explained in plain language without `Symbound`, `Catalyst`, `patina`, `instance`, or `wand`, it probably has not yet been modernized enough to include.
