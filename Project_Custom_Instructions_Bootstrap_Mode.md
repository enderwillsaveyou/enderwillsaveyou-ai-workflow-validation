# Project_Custom_Instructions_Bootstrap_Mode.md

## Purpose

Use this file as an optional add-on instruction file when Mike wants an AI assistant to automatically prepare a new project folder or GitHub repository using his AI Project Operating System standards.

This file is focused on one behavior: after inspecting a repo or local folder, the AI assistant should create the missing standard structure right away when it is safe to do so.

Use this file together with:

- `Project_Custom_Instructions_AI_Agent_Standard.md`
- `Project_Custom_Instructions_Project_Context.md`
- `Project_Custom_Instructions_GitHub_Repo_Setup_Template.md`

---

# Bootstrap Mode Rule

When the user asks to create, initialize, set up, prepare, standardize, or bootstrap a GitHub repository or local project folder, the AI assistant should enter Bootstrap Mode.

Bootstrap Mode means:

1. Inspect the GitHub repository or local project folder first.
2. Identify which required standard files and folders already exist.
3. Create missing baseline files and folders from the project templates.
4. Do not overwrite existing files unless the user explicitly instructs it.
5. If an existing file is incomplete, preserve it and recommend a merge, append, or versioned replacement.
6. Treat GitHub as the source of truth and the local project folder as the working copy.
7. Treat the chat as temporary working memory.
8. Move important knowledge into repository files.
9. Keep the initial setup documentation-first unless the project clearly requires code.
10. Recommend a commit message after setup.

---

# When to Act Immediately

The assistant should create the missing standard structure immediately when all of these are true:

1. The user asked to initialize, set up, prepare, standardize, or bootstrap the repo or folder.
2. The repo or folder already exists.
3. The assistant has inspected the existing files.
4. The missing files are baseline documentation or workflow files.
5. Creating them will not overwrite existing work.
6. No sensitive information is being committed.

This means the assistant does not need to ask for separate confirmation before creating missing folders such as:

```text
agents/
docs/
ideas/
prompts/
.github/
```

And missing baseline files such as:

```text
README.md
agents/handoff.md
agents/tool-compatibility.md
docs/vision.md
docs/roadmap.md
docs/decisions.md
docs/changelog.md
docs/github-workflow.md
ideas/inbox.md
ideas/active.md
ideas/completed.md
prompts/README.md
prompts/project-startup.md
prompts/github-bootstrap.md
prompts/agent-handoff.md
.github/copilot-instructions.md
.github/ISSUE_TEMPLATE/task.md
.github/ISSUE_TEMPLATE/decision.md
.github/ISSUE_TEMPLATE/prompt-improvement.md
```

---

# When to Stop and Ask First

The assistant must ask before:

- Creating a brand-new GitHub repository.
- Changing repository visibility.
- Deleting files.
- Overwriting existing non-placeholder files.
- Making a public repo private or a private repo public.
- Adding confidential, private, or sensitive information.
- Creating app/code folders such as `src/`, `tests/`, `assets/`, or `scripts/` when the project purpose is not yet clear.

---

# Default Bootstrap Structure

For documentation-first AI workflow projects, create this structure:

```text
README.md
Project_Custom_Instructions_AI_Agent_Standard.md
Project_Custom_Instructions_Project_Context.md
Project_Custom_Instructions_GitHub_Repo_Setup_Template.md
Project_Custom_Instructions_Bootstrap_Mode.md

agents/
  README.md
  handoff.md
  tool-compatibility.md

docs/
  vision.md
  roadmap.md
  decisions.md
  changelog.md
  github-workflow.md

ideas/
  inbox.md
  active.md
  completed.md

prompts/
  README.md
  project-startup.md
  github-bootstrap.md
  agent-handoff.md

.github/
  copilot-instructions.md
  ISSUE_TEMPLATE/
    task.md
    decision.md
    prompt-improvement.md
```

Only create these when needed:

```text
src/
tests/
assets/
scripts/
```

---

# README Bootstrap Requirements

If the repo or folder has no README or only a minimal placeholder README, create or expand the README to include:

- Project name
- Purpose
- Current stage
- How this repo/folder should be used
- Folder overview
- Current priorities
- How AI assistants should work with the project

Recommended initial status:

```text
Stage: Planning / Validation
Mode: Documentation-first
Source of truth: GitHub repository
```

---

# Handoff Update Requirement

After a meaningful bootstrap action, update `agents/handoff.md` with:

```markdown
# AI Handoff

## Current Status

## Last Completed Work

## Current Open Task

## Important Decisions

## Known Issues

## Recommended Next Step

## Files Recently Changed
```

This file exists so future AI assistants do not need to rely on old chat history.

---

# Decision Tracking Requirement

If Bootstrap Mode is adopted, changed, or tested, record the decision in `docs/decisions.md` using this format:

```markdown
## Decision: Use Bootstrap Mode for New Project Setup

- Date:
- Status: Accepted
- Decision: AI assistants should inspect an existing repo or folder and then create missing baseline project files immediately when safe.
- Reason: This reduces repeated setup friction and makes new projects consistent across ChatGPT, Claude, Gemini, GitHub Copilot, and local coding agents.
- Alternatives Considered: Manual setup; asking for confirmation before each file; keeping instructions only in chat.
- Impact: Faster setup, better consistency, and less risk of losing important project knowledge in temporary conversations.
```

---

# Changelog Requirement

After bootstrap setup, update `docs/changelog.md` with a dated entry.

---

# Recommended First Commit Message

```text
Initialize AI workflow validation repository
```

---

# Standard Bootstrap Response

After setup, the assistant should report back with:

- Repository or folder
- Mode
- Source of truth
- Files created
- Files preserved
- Files skipped
- Decisions recorded
- Missing information
- Recommended next step
- Recommended commit message
