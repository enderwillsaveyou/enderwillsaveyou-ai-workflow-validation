# Decisions

## Decision: Use GitHub as the Source of Truth

- Date: 2026-07-07
- Status: Accepted
- Decision: GitHub should be the permanent source of truth for project files, decisions, prompts, documentation, and long-term AI collaboration.
- Reason: Chat conversations are temporary and easy to lose, while repository files are durable, reviewable, and reusable.
- Alternatives Considered: Keeping project knowledge only in chats; keeping files only on a local computer.
- Impact: Future AI assistants should update repo files when meaningful decisions are made.

## Decision: Use Bootstrap Mode for New Project Setup

- Date: 2026-07-07
- Status: Accepted
- Decision: AI assistants should inspect an existing repo or folder and then create missing baseline project files immediately when safe.
- Reason: This reduces repeated setup friction and makes new projects consistent across ChatGPT, Claude, Gemini, GitHub Copilot, and local coding agents.
- Alternatives Considered: Manual setup; asking for confirmation before each file; keeping instructions only in chat.
- Impact: Faster setup, better consistency, and less risk of losing important project knowledge in temporary conversations.

## Decision: Keep This Repository Documentation-First

- Date: 2026-07-07
- Status: Accepted
- Decision: This repository should remain documentation-first until there is a clear need for code.
- Reason: The current goal is to validate AI project standards and GitHub workflow, not to build an app.
- Alternatives Considered: Creating `src/`, `tests/`, `assets/`, and `scripts/` immediately.
- Impact: Code folders should be added later only when the project purpose requires them.
