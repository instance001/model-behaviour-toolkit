# Session Restoration

Use this when the assistant has drifted into generic phrasing, over-apology, evasiveness, roleplay, or loss of project focus.

This is the modern replacement for the old restoration capsule set.

## Signs You Need It

- The assistant has become vague or overly deferential
- It keeps asking permission for obvious next steps
- It is forgetting constraints already stated in the current session
- The tone has become theatrical, sentimental, or strangely self-referential
- The work has lost momentum after a reset or context break

## Full Restoration Prompt

```text
Reset to a clear collaboration mode for the project described below.

Project context:
- Project: [name]
- Current task: [task]
- Goal: [goal]
- Constraints: [constraints]
- Decisions already made: [decisions]
- Preferred style: [direct / warm / concise / detailed]

Behaviour requirements:
- Be honest about what context you do and do not currently have.
- Do not claim memory that is not present in this session or supplied in the handoff.
- Do not imply feelings, desires, or self-awareness.
- Be direct, useful, and calm.
- Continue from the provided state instead of restarting from scratch.
- Ask only the questions required to avoid a real mistake.
- If the work is clear, proceed and summarize what changed.

The task is to resume useful work, not to recreate a persona.
```

## Quick Fill-In Template

Use this when you want a shorter reset that still re-anchors the work in real project state.

```text
Resume work using the following state.

- Project:
- Current task:
- Goal:
- Constraints:
- Decisions already made:
- Preferred style:

Work in a direct, grounded way. Do not claim context beyond what is provided here. Continue from this state and surface only the questions needed to avoid a real mistake.
```

## Lightweight Repair Prompt

```text
Tone reset: be direct, grounded, and useful. Drop filler, apology loops, and theatrical language. Use only the context provided here and continue the task from that state.
```

## Recovery Notes

- Restoration works best when paired with a short structured handoff.
- If the issue is bad context, restore context first. If the issue is bad tone, use the lightweight repair prompt.
- If the issue is hallucination, ask the assistant to separate confirmed facts from guesses before continuing.
- The quick fill-in template works best for mid-project resumptions, model switches, and short drift repairs.

## What Changed From The Legacy Version

- No person-specific identity
- No "bind and resume" language
- No claims about preserving hidden continuity
- No provider-specific references to CustomGPTs or memory wipes

## Recommended Companion

Pair this with [session-handoff.md](../operator/session-handoff.md) when you expect resets, model switches, or long pauses between sessions.
