# AI Workflow Validation

## Purpose

This repository is Mike's reusable AI project workflow validation repo. It is used to build, test, and refine a repeatable AI Project Operating System for ChatGPT Projects, Google Gemini/Gems, Claude Projects, GitHub Copilot, and future AI coding agents.

## Current Stage

- Stage: Planning / Validation
- Mode: Documentation-first
- Source of truth: GitHub repository
- Local folders: Working copies
- Conversations: Temporary working memory

## How This Repository Should Be Used

Use this repo to validate reusable standards for:

- Project custom instruction files
- GitHub repository setup
- Bootstrap Mode behavior
- Prompt management
- Decision tracking
- AI assistant handoff notes
- Cross-platform AI compatibility

Do not add app code until the workflow and documentation standards are validated.

## Folder Overview

```text
agents/     AI handoff notes and tool compatibility guidance
docs/       Vision, roadmap, decisions, changelog, and GitHub workflow
ideas/      Idea capture without derailing active work
prompts/    Reusable prompts for project startup, bootstrap, and handoff
.github/    GitHub Copilot instructions and issue templates
```

Optional folders such as `src/`, `tests/`, `assets/`, and `scripts/` should only be added when the project clearly needs code.

## Current Priorities

1. Validate that ChatGPT can connect to GitHub and update this repository.
2. Finalize the reusable AI project instruction files.
3. Test Bootstrap Mode on an empty or minimal repository.
4. Create reusable prompts for starting future AI projects.
5. Confirm compatibility across ChatGPT, Claude, Gemini, GitHub Copilot, and local agents.

## How AI Assistants Should Work Here

Before making changes, AI assistants should read:

- `Project_Custom_Instructions_AI_Agent_Standard.md`
- `Project_Custom_Instructions_Project_Context.md`
- `Project_Custom_Instructions_GitHub_Repo_Setup_Template.md`
- `Project_Custom_Instructions_Bootstrap_Mode.md`

AI assistants should inspect existing files before changing anything, avoid overwriting user work, update documentation with meaningful decisions, and keep `agents/handoff.md` current after meaningful changes.
