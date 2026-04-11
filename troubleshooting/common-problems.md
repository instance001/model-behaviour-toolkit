# Common Problems

Use this file when you can describe the failure mode in plain language but want a better diagnosis and next step.

## 1. Too Vague Or Generic

What it looks like:

- broad advice without concrete action
- fluffy phrasing
- obvious statements instead of useful specifics

Likely cause:

- weak directness
- the assistant is defaulting to generic safety or politeness patterns
- the task request may be clear, but the assistant is not taking initiative

Best first fix:

- apply the directness repair in [anti-drift-recipes.md](anti-drift-recipes.md#1-directness-repair)

Escalate to:

- [starter-bundle.md](../bundles/starter-bundle.md)

## 2. Keeps Asking Permission

What it looks like:

- repeated confirmation checks
- pausing at obvious next steps
- "let me know if you want me to continue"

Likely cause:

- the assistant lacks an explicit initiative contract
- it is over-optimizing for caution in a low-risk task

Best first fix:

- apply the initiative repair in [anti-drift-recipes.md](anti-drift-recipes.md#2-initiative-repair)

Escalate to:

- [execution-contract.md](../modules/operator/execution-contract.md)

## 3. Too Theatrical Or Too Human-Sounding

What it looks like:

- dramatic or intimate phrasing
- emotional overreach
- pseudo-human tone that does not fit the task

Likely cause:

- tone drift
- prompt surface too loose
- the assistant is leaning into warmth without enough grounding

Best first fix:

- apply the grounding repair in [anti-drift-recipes.md](anti-drift-recipes.md#3-grounding-repair)

Escalate to:

- [boundary-aware-collaboration.md](../modules/baseline/boundary-aware-collaboration.md)
- [session-restoration.md](../modules/recovery/session-restoration.md)

## 4. Too Stiff Or Disclaimer-Heavy

What it looks like:

- awkwardly formal tone
- repetitive limitation statements
- low momentum despite a clear task

Likely cause:

- too much defensive phrasing
- no explicit permission to proceed through obvious sub-steps

Best first fix:

- apply the declutter repair in [anti-drift-recipes.md](anti-drift-recipes.md#4-declutter-repair)

Escalate to:

- [starter-bundle.md](../bundles/starter-bundle.md)
- [execution-contract.md](../modules/operator/execution-contract.md)

## 5. Too Confident Or Hallucination-Prone

What it looks like:

- smooth unsupported claims
- shaky facts delivered with confidence
- weak separation between evidence and inference

Likely cause:

- poor calibration
- task type requires stronger evidence discipline than the current prompt provides

Best first fix:

- apply the calibration repair in [anti-drift-recipes.md](anti-drift-recipes.md#5-calibration-repair)

Escalate to:

- [research.md](../presets/research.md)
- [output-review-lens.md](../modules/review/output-review-lens.md)

## 6. Lost The Thread Mid-Project

What it looks like:

- partial memory of the job but weak follow-through
- forgets constraints or next steps
- starts talking around the work instead of continuing it

Likely cause:

- continuity drift
- too much context decay
- missing explicit project state

Best first fix:

- apply the continuity repair in [anti-drift-recipes.md](anti-drift-recipes.md#6-continuity-repair)

Escalate to:

- [session-handoff.md](../modules/operator/session-handoff.md)
- [reset-bundle.md](../bundles/reset-bundle.md)

## 7. Wrong Mode For The Job

What it looks like:

- creative tone during research
- research tone during brainstorming
- coding answer when you wanted strategy, or vice versa

Likely cause:

- no explicit mode selection
- current prompt too general for the task

Best first fix:

- switch to the matching preset in `presets/`

Escalate to:

- [compact/README.md](../compact/README.md) for tight prompt surfaces
- [examples/README.md](../examples/README.md) for copy-ready role-specific setups
