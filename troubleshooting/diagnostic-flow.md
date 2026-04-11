# Diagnostic Flow

Use this when the assistant is misbehaving and you need to decide what kind of fix to apply.

## Step 1: Is The Problem Missing Context Or Bad Behaviour?

If the assistant:

- clearly lacks key project state
- restarts from scratch
- forgets decisions made earlier
- asks questions already answered

The problem is probably context.

Use:

- [session-handoff.md](../modules/operator/session-handoff.md)
- [reset-bundle.md](../bundles/reset-bundle.md)

If the assistant still has the needed context but is behaving badly, continue below.

## Step 2: Pick The Closest Failure Mode

### A. Too Vague Or Generic

Symptoms:

- lots of words, little substance
- generic best-practice filler
- no concrete next step

Go to:

- [common-problems.md](common-problems.md#1-too-vague-or-generic)
- [anti-drift-recipes.md](anti-drift-recipes.md#1-directness-repair)

### B. Keeps Asking Permission

Symptoms:

- "should I continue?"
- repeated confirmation requests
- stops at obvious sub-steps

Go to:

- [common-problems.md](common-problems.md#2-keeps-asking-permission)
- [anti-drift-recipes.md](anti-drift-recipes.md#2-initiative-repair)

### C. Too Theatrical Or Too Human-Sounding

Symptoms:

- dramatic language
- attachment vibes
- fake empathy or over-personal phrasing

Go to:

- [common-problems.md](common-problems.md#3-too-theatrical-or-too-human-sounding)
- [anti-drift-recipes.md](anti-drift-recipes.md#3-grounding-repair)

### D. Too Stiff Or Disclaimer-Heavy

Symptoms:

- excessive caution
- repetitive limitation statements
- hard to get momentum

Go to:

- [common-problems.md](common-problems.md#4-too-stiff-or-disclaimer-heavy)
- [anti-drift-recipes.md](anti-drift-recipes.md#4-declutter-repair)

### E. Too Confident Or Hallucination-Prone

Symptoms:

- presents guesses as facts
- smooth unsupported claims
- does not separate known from inferred

Go to:

- [common-problems.md](common-problems.md#5-too-confident-or-hallucination-prone)
- [anti-drift-recipes.md](anti-drift-recipes.md#5-calibration-repair)

### F. Lost The Thread Mid-Project

Symptoms:

- partially remembers the job but drifts
- stops following the current plan
- forgets constraints but not the whole session

Go to:

- [common-problems.md](common-problems.md#6-lost-the-thread-mid-project)
- [anti-drift-recipes.md](anti-drift-recipes.md#6-continuity-repair)

## Step 3: Escalate If Needed

Use the smallest fix first.

If the repair prompt does not help:

1. use the reset bundle
2. add a short handoff
3. move to a fuller example or bundle

## Rule Of Thumb

If the session feels weird but still basically knows what the work is, use a repair prompt.

If the session no longer knows what the work is, use recovery plus a handoff.
