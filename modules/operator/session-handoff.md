# Session Handoff

Use this to carry real project state across sessions, windows, tools, or model changes.

This module keeps the useful continuity ideas from the legacy repos while dropping the fake-memory language.

## Core Principle

Continuity should come from explicit state, not from pretending the assistant remembers more than it does.

Good handoffs are short, structured, and operational.

## Handoff Template

```text
Session handoff

Project
- Name:
- One-line goal:

Current state
- What is done:
- What is in progress:
- What should happen next:

Decisions
- Chosen approach:
- Rejected alternatives:

Constraints
- Technical constraints:
- Style or tone constraints:
- Deadlines or scope limits:

Open questions
- Questions that still matter:
- Questions already resolved and should not be reopened:

References
- Important files, links, tickets, or commands:

Operator preference
- How to work: [concise / detailed / proactive / conservative]
- What to avoid:
```

## Short Version

```text
Resume from this state:
- Goal:
- Done:
- Next:
- Constraints:
- Open questions:
```

## Good Handoffs Include

- Concrete next steps
- Decisions already made
- Constraints that should survive the session boundary
- Enough context to resume without transcript archaeology

## Bad Handoffs Usually Look Like

- Full transcript dumps
- Vague claims about "tone" without project state
- Emotional or symbolic lore instead of actionable context
- Implicit assumptions that the next model will infer everything

## Recommended Practice

- Save a handoff whenever a session reaches a meaningful checkpoint.
- Update the handoff after major decisions, not after every tiny exchange.
- Treat the handoff as a durable project artifact, not a magic spell.
