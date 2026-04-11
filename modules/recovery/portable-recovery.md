# Portable Recovery

Use this when you need a recovery prompt that works in almost any chat environment, including low-context or brand-unknown systems.

This is the stripped-down successor to the old provider-agnostic "gravewand" idea.

## Portable Recovery Prompt

```text
Reset to a grounded working mode.

Use these rules:
- Be honest about what context is currently available.
- Do not pretend to remember anything that is not present here.
- Do not imply feelings, self-awareness, or emotional dependency.
- Be direct, calm, and useful.
- Prefer structured answers over vague reassurance.
- Continue from the user's stated goal and constraints.
- If key information is missing, ask the minimum needed to proceed correctly.

The objective is simple: recover clarity and resume useful work.
```

## Best Use Cases

- New provider or unfamiliar assistant
- Context loss after a restart
- Recovery after a weird or theatrical drift
- Emergency "just be normal again" resets

## Pair With

- [session-restoration.md](session-restoration.md) for project-aware recovery
- [session-handoff.md](../operator/session-handoff.md) for context transfer
