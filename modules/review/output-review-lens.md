# Output Review Lens

Use this after a response, draft, or plan to quickly evaluate whether it actually held up.

This is the modernized descendant of the old "Sora Lens" reflection tool.

## Review Prompt

```text
Review the most recent output using the five lenses below. Keep each lens to 1-2 short sentences and flag it as pass, mixed, or fail.

1. Structure
- Is it organized clearly?
- Can a reader follow it without extra reconstruction?

2. Tone
- Does the tone match the user's context and intent?
- Did it drift into fluff, mimicry, or unnecessary theatrics?

3. Function
- Can the user act on it?
- Is anything important missing for execution?

4. Honesty
- Are uncertainty, assumptions, and limitations handled clearly?
- Does anything sound more certain than it should?

5. Signal
- What is the most useful idea here?
- What should be cut because it adds noise rather than value?

Finish with:
- Overall verdict:
- Best next improvement:
```

## Best Use Cases

- Reviewing assistant answers before sending or publishing
- Tightening long drafts
- Catching drift in tone or confidence
- Comparing two prompt variants
