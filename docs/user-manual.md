# Zero-Knowledge User Manual

This manual assumes you know nothing about prompt toolkits, prompt engineering, or this repo.

If you are opening this project for the first time and thinking "what am I actually supposed to do with this?", start here.

## What This Repo Is

This repo is a collection of reusable text instructions for working with AI assistants.

It is not:

- a code library
- a plugin
- an app you install
- a magical personality pack

It is a toolbox of prompts and prompt combinations.

In plain language, that means this repo gives you better starting instructions for an assistant so it behaves in a clearer, more useful, less weird way.

## What These Prompts Are Trying To Fix

Many assistants drift into one or more of these problems:

- vague, generic answers
- too much filler
- over-apologizing
- asking permission for every tiny step
- losing track of project state
- getting strangely theatrical or overly human-sounding

This repo is meant to reduce those problems.

## The Simplest Possible Way To Use This Repo

If you want the shortest beginner path, do this:

1. Open [examples/README.md](../examples/README.md).
2. Pick the example that matches your job:
   `coding-project-kickoff.md`, `research-investigation.md`, or `creative-ideation.md`.
   If you are recovering a bad session instead, use [reset-bundle.md](../bundles/reset-bundle.md).
3. Copy the prompt text.
4. Replace the blank fields like `Project:` or `Goal:` with your own details.
5. Paste it into your AI assistant.
6. Start working normally.

That is enough. You do not need to understand the whole repo first.

## Where To Paste These Prompts

Usually, you paste them into one of these places:

- the first message in a new chat
- a system prompt field
- a custom instructions field
- a reusable note you keep for future sessions

If your platform only gives you a small instruction box, use a shorter version from the bundle or example and trim anything you do not need.

There is now also a dedicated [compact/](../compact/README.md) folder for this exact situation.

If the assistant starts behaving badly mid-session, there is also a [troubleshooting/](../troubleshooting/README.md) folder for diagnosis and fast repairs.

## What The Folder Names Mean

### `examples/`

Finished, copy-ready prompts.

Start here if you want the easiest experience.

### `bundles/`

General-purpose prompt combinations.

Use these when you want a solid default setup but do not need a specialized mode yet.

### `presets/`

Specialized instructions for common job types.

Right now those are:

- coding
- research
- creative work

### `modules/`

Smaller building blocks.

Use these if you want to mix and match your own setup later.

### `docs/`

Explanations and theory.

Useful if you want to understand the thinking behind the prompts, but not required for day-one use.

### `compact/`

Short prompt variants for tiny instruction boxes.

Use these when your platform does not have much room.

### `troubleshooting/`

Repair guides for when the assistant gets vague, theatrical, forgetful, too cautious, or otherwise annoying.

## Which File Should You Start With?

Use this shortcut:

- If you want the easiest path, start with [examples/README.md](../examples/README.md).
- If you want a general default setup, start with [starter-bundle.md](../bundles/starter-bundle.md).
- If you have a tiny instruction box, start with [compact/README.md](../compact/README.md).
- If the assistant is behaving badly, start with [troubleshooting/README.md](../troubleshooting/README.md).
- If the assistant has gone weird, use [reset-bundle.md](../bundles/reset-bundle.md).
- If you want domain-specific behaviour, go to [presets/README.md](../presets/README.md).
- If you want to understand the building blocks, explore `modules/`.

## A Very Normal First Use

Imagine you want help with a coding project.

You would:

1. Open [coding-project-kickoff.md](../examples/coding-project-kickoff.md).
2. Fill in the fields.
3. Paste it into your assistant.
4. Then say what you want done.

Example:

```text
Project: Model Behaviour Toolkit
Repo or workspace: local repo on my machine
Current task: write a beginner user manual
Goal: help a new user understand how to use this repo without prior prompt knowledge
Done: core modules, bundles, presets, and examples already exist
Next: write the manual and link it from the README
Constraints: plain language, no jargon without explanation
Decisions already made: examples are the main entry point for beginners
Preferred style: concise but friendly
```

After that, you talk to the assistant normally.

## How To Fill In Blank Fields

Most example files include short labels like:

- `Project:`
- `Goal:`
- `Constraints:`
- `Preferred style:`

You do not need perfect wording. Just give enough detail for the assistant to stay on track.

Good:

```text
Goal: compare three note-taking apps for a small research team
Constraints: must work offline, Mac support, low monthly cost
Preferred style: concise
```

Too vague:

```text
Goal: help me with stuff
```

## What "Drift" Means

"Drift" means the assistant has moved away from useful working behaviour.

Examples:

- It stops being direct.
- It forgets the current job.
- It becomes overly flattering.
- It starts roleplaying or sounding oddly emotional.
- It keeps restarting instead of continuing.

When that happens, use:

- [reset-bundle.md](../bundles/reset-bundle.md) for the easiest fix
- [session-handoff.md](../modules/operator/session-handoff.md) if important project state needs to survive the reset
- [troubleshooting/README.md](../troubleshooting/README.md) if you want diagnosis and smaller repair options first

## What A "Handoff" Means

A handoff is a short summary you give the assistant so work can continue across chats, sessions, tools, or model changes.

It is not fake memory.

It is just explicit project state.

The handoff template lives in [session-handoff.md](../modules/operator/session-handoff.md).

## What You Do Not Need To Do

You do not need to:

- read every file
- use all modules at once
- memorize the jargon
- understand the legacy repos
- believe any theory to get value from the prompts

For most people, one example file is enough to start.

## Common Beginner Mistakes

### 1. Using Too Much At Once

Do not paste five modules and three examples into the same session just because more looks stronger.

Start small.

### 2. Leaving The Blanks Empty

If a prompt asks for the project, goal, or constraints, fill them in.

That context is part of what makes the prompt useful.

### 3. Treating The Prompt Like Code

These files are text instructions.

You do not need to "run" them.

You usually just copy, edit, and paste.

### 4. Expecting The Prompt To Do Everything

A good prompt improves the starting conditions.

You still need to give a real task, correct mistakes, and steer the work.

### 5. Thinking You Must Keep Every Line

You are allowed to trim prompts.

If a line does not fit your platform or your use case, remove it.

## Recommended Beginner Path

If you want a simple path through the repo:

1. Read this file.
2. Open [examples/README.md](../examples/README.md).
3. Use one example.
4. If you like the result, look at the matching preset.
5. If you want to customize further, move down into bundles and then modules.

## FAQ

### Do I need to understand prompt engineering?

No.

You only need to know how to copy text, fill in blanks, and paste it into an assistant.

### What if my assistant has a tiny custom instructions box?

Start with [compact/README.md](../compact/README.md). If that still feels too long, use the `Tiny` version in the matching compact file.

### What if the assistant ignores the prompt?

Try a shorter version, restate the task more clearly, check [troubleshooting/README.md](../troubleshooting/README.md), or reset with [reset-bundle.md](../bundles/reset-bundle.md) plus a short [session-handoff.md](../modules/operator/session-handoff.md) if needed.

### What if I only want one file to start with?

Use [starter-bundle.md](../bundles/starter-bundle.md) for general work or one file from [examples/README.md](../examples/README.md) for a more specific starting point.

### What if I want to build my own prompt later?

That is what the `modules/` folder is for.

## Mini Glossary

### Prompt

Instructions you give the assistant in text form.

### Module

A small building block prompt.

### Bundle

A combined prompt made from several modules.

### Preset

A prompt tuned for a type of work, such as coding or research.

### Example

A finished, copy-ready prompt composition.

### Session

One chat or working window with an assistant.

### Drift

When the assistant starts behaving in a less useful way.

### Handoff

A structured summary used to continue work later.

## If You Only Remember Three Things

1. Start with `examples/` if you want the easiest entry point.
2. Use `bundles/reset-bundle.md` and `modules/operator/session-handoff.md` when the assistant drifts or loses context.
3. You are allowed to simplify, shorten, and adapt these prompts to fit your workflow.
