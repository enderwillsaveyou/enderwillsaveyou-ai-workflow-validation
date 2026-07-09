# Roadmap

## Phase 1 — Validate AI Project Standards

- Confirm the instruction files make sense.
- Confirm ChatGPT can read uploaded project files.
- Confirm ChatGPT can connect to GitHub and update the repo.

## Phase 2 — Finalize Template Files

- Refine the AI agent standard.
- Refine the project context template.
- Refine the GitHub setup template.
- Refine Bootstrap Mode.

## Phase 3 — Test GitHub Workflow from AI Chat

- Create or update files through the GitHub connector.
- Validate safe inspection-before-editing behavior.
- Track meaningful decisions in `docs/decisions.md`.

## Phase 4 — Test Cross-Platform AI Compatibility

- Test the same files in ChatGPT Projects.
- Test the same files in Claude Projects.
- Test the same files in Google Gemini/Gems.
- Test the same repo with GitHub Copilot.

## Phase 5 — Use Template on a Real Project

- Create a new project using this standard.
- Upload the instruction files.
- Connect or create a repo.
- Run Bootstrap Mode.
- Compare results across tools.

## Phase 6 — Define Ender v0

Goal: Establish Ender as the conversational front-end and coordinator layer for the AI OS.

Ender v0 should focus on coordination, not autonomous coding.

Initial responsibilities:

- Use ChatGPT Projects as the conversational workspace for brainstorming, planning, and project direction.
- Keep GitHub as the permanent source of truth for project state, decisions, ideas, prompts, and handoffs.
- Capture new ideas from chat and route them into the correct repository file.
- Move approved ideas into `ideas/active.md`.
- Record architecture and workflow decisions in `docs/decisions.md`.
- Keep `agents/handoff.md` updated so Codex, Claude Code, Gemini Antigravity, and future coding agents can continue from the current state.
- Prepare clear implementation prompts for coding agents.
- Review coding-agent outputs and capture follow-up work.

Next steps:

1. Define the Ender v0 role and boundaries.
2. Create or update a dedicated Ender instruction file.
3. Define routing rules for ideas, decisions, prompts, handoffs, and roadmap updates.
4. Test the workflow by discussing an idea in ChatGPT, updating repository documentation, and handing it off to a coding agent.
5. Decide whether Ender belongs in this validation repo first or in the main AI OS repo.
