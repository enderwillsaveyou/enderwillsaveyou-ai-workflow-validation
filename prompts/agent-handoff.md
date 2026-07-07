# Agent Handoff Prompt

## Purpose

Use this prompt when an AI assistant needs to summarize current project state for the next assistant.

## Best Used With

- ChatGPT Projects
- Claude Projects
- Gemini/Gems
- GitHub-connected coding agents
- Local coding agents

## Inputs Needed

- Current repo or folder state
- Recent changes
- Open questions
- Recommended next step

## Prompt

```text
Create or update `agents/handoff.md` so a future AI assistant can continue without relying on old chat history.

Include:

- Current status
- Last completed work
- Current open task
- Important decisions
- Known issues
- Recommended next step
- Files recently changed

Keep it concise and factual.
```

## Expected Output

A complete update to `agents/handoff.md`.

## Notes

Use this after meaningful repo or project changes.

## Version

1.0
