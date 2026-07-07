# Project_Custom_Instructions_GitHub_Repo_Setup_Template.md

## Purpose

Use this file when an AI assistant is asked to create, initialize, inspect, bootstrap, or manage a GitHub repository for a project that follows Mike's AI Project Operating System standards.

This file is focused only on GitHub repository setup, local project folder setup, and GitHub-based project management. It should be used together with:

- `Project_Custom_Instructions_AI_Agent_Standard.md`
- `Project_Custom_Instructions_Project_Context.md`
- `Project_Custom_Instructions_Bootstrap_Mode.md`

The goal is to make GitHub the permanent source of truth for project files, decisions, prompts, documentation, and long-term AI collaboration.

---

# Core Rule

Do not assume a GitHub repository already exists.

Before doing GitHub work, confirm whether the project already has a repository.

If the repository exists, inspect it before changing anything.

If the repository does not exist, follow the repository creation workflow.

If the user asks to initialize, set up, prepare, or bootstrap an existing repository or local project folder, inspect first and then create the missing standard structure immediately, as long as doing so does not overwrite existing work.

---

# Bootstrap Mode

Bootstrap Mode is the default setup behavior when the user asks an AI assistant to create, initialize, set up, prepare, standardize, or bootstrap a GitHub repository or local project folder.

Bootstrap Mode means:

1. Inspect the GitHub repository or local project folder first.
2. Identify which required standard files and folders already exist.
3. Create any missing baseline files and folders from this template.
4. Do not overwrite existing files unless the user explicitly instructs it.
5. If a file already exists but is incomplete, preserve it and recommend either appending, merging, or creating a versioned replacement.
6. Treat GitHub as the source of truth and the local project folder as the working copy.
7. Keep the initial setup documentation-first unless the project clearly requires code.
8. Create `src/`, `tests/`, `assets/`, and `scripts/` only when the project needs them.
9. Update `agents/handoff.md`, `docs/changelog.md`, and `docs/decisions.md` when meaningful setup decisions are made.
10. Recommend a small, descriptive commit message after setup.
11. Recommend starter issues or pull requests when useful.

No extra confirmation is required to create missing baseline documentation files when all of these are true:

1. The user has asked to initialize, set up, prepare, standardize, or bootstrap the repo or folder.
2. The repo or folder already exists.
3. The files being created are missing.
4. The action does not delete or overwrite existing work.
5. No sensitive information is being committed.

Confirmation is required before:

- Creating a new GitHub repository.
- Changing repository visibility.
- Deleting files.
- Overwriting existing non-placeholder files.
- Committing confidential, private, or sensitive information.
- Creating public repositories that may contain personal, work, or sensitive project information.

---

# Repository Setup Checklist

Before creating or initializing a repository, confirm or derive:

- GitHub owner or organization
- Repository name
- Repository full name, such as `owner/repo-name`
- Visibility
- Default branch
- Project name
- Project purpose
- Initial project stage
- Whether the repository is documentation-only, code-based, or mixed
- Whether the repository should be used as a reusable template
- Whether issues, labels, and GitHub project tracking should be initialized

Default recommendation for new personal AI workflow projects:

```text
Visibility: private
Default branch: main
Initial mode: documentation-first
Repository type: reusable workflow/template foundation
```

---

# Repository Inspection Rules

If the repository already exists, inspect before modifying.

Check for:

- Existing README
- Existing project context file
- Existing AI instruction files
- Existing docs folder
- Existing prompts folder
- Existing ideas folder
- Existing agents folder
- Existing `.github` folder
- Existing issues
- Existing branches
- Existing GitHub Actions workflows
- Existing codebase

Do not overwrite existing files unless explicitly instructed.

Prefer merging, appending, or creating a new versioned file.

If the repo is empty or nearly empty and the user asked for setup, enter Bootstrap Mode and create the missing standard structure immediately.

---

# Initial Repository Structure

For a new AI workflow/template repository, initialize this structure:

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

Only create `src/`, `tests/`, `assets/`, and `scripts/` when the project requires them.

---

# Required Initial Files

## README.md

Purpose: Front door of the repository.

Include:

- Project name
- Purpose
- Current stage
- How this repo should be used
- Folder overview
- Current priorities
- How AI assistants should work with the repo

## Project_Custom_Instructions_AI_Agent_Standard.md

Purpose: Reusable AI operating standard.

Do not bury project-specific details in this file.

## Project_Custom_Instructions_Project_Context.md

Purpose: Project-specific context.

Include project name, purpose, vision, target users, technology stack, current status, success criteria, constraints, current priorities, known issues, important links, notes for AI assistants, and repository setup details.

## agents/handoff.md

Purpose: Help future AI assistants continue work without relying on old chat history.

Update this file after meaningful project changes.

## docs/decisions.md

Purpose: Record important project decisions.

Use this format:

```markdown
## Decision: <Title>

- Date:
- Status: Proposed / Accepted / Replaced / Deprecated
- Decision:
- Reason:
- Alternatives Considered:
- Impact:
```

## docs/changelog.md

Purpose: Track meaningful changes.

Use this format:

```markdown
# Changelog

## YYYY-MM-DD

### Added

### Changed

### Fixed

### Removed
```

## docs/github-workflow.md

Purpose: Explain how GitHub should be used for this project.

Include branch strategy, commit strategy, issue workflow, pull request expectations, documentation update rules, AI assistant workflow, Bootstrap Mode behavior, and source-of-truth handling.

---

# GitHub Issue Setup

If the AI tool can create GitHub issues, create starter issues after the repo is initialized.

Recommended starter issues:

1. Finalize AI Agent Standard v2
2. Finalize Project Context Template v2
3. Create GitHub bootstrap prompt
4. Create prompt tracking workflow
5. Create decision tracking workflow
6. Test ChatGPT to GitHub file creation workflow
7. Test Claude compatibility workflow
8. Test Gemini compatibility workflow
9. Document first successful AI-assisted GitHub workflow
10. Validate Bootstrap Mode on a new repo
11. Validate Bootstrap Mode on an existing minimal repo
12. Validate local project folder bootstrap workflow

---

# Recommended Labels

If labels can be created or managed, use these:

```text
documentation
prompt
workflow
github
ai-agent
decision
idea
template
testing
bootstrap
local-folder
blocked
needs-review
```

If label creation is not available, list the recommended labels in `docs/github-workflow.md`.

---

# Branch Strategy

For solo personal workflow projects, keep branching simple.

Default branch:

```text
main
```

Optional working branches:

```text
docs/<topic>
prompts/<topic>
workflow/<topic>
fix/<topic>
bootstrap/<topic>
```

---

# Commit Strategy

Use small, descriptive commits.

Good examples:

```text
Initialize AI workflow validation repository
Add GitHub repository setup template
Add Bootstrap Mode instructions
Add project context template
Document decision tracking workflow
Add prompt management structure
Update AI agent standard with repo bootstrap rules
```

Avoid vague commit messages.

---

# Pull Request Strategy

For a personal learning repo, pull requests are optional but useful for practicing workflow.

Use pull requests when:

- Testing AI-assisted GitHub workflows
- Reviewing larger documentation changes
- Changing the project standard
- Adding reusable templates
- Testing collaboration between multiple AI assistants

---

# Prompt Management Workflow

When the user creates or improves a prompt:

1. Decide whether it is reusable.
2. If reusable, save it under `prompts/`.
3. Include purpose, target tool, inputs, expected output, and notes.
4. Update changelog if the prompt is important.
5. Recommend a commit message.

---

# Decision Tracking Workflow

When a meaningful decision is made:

1. Summarize the decision.
2. Explain the reason.
3. Note alternatives considered.
4. Add it to `docs/decisions.md`.
5. Update `agents/handoff.md` if future assistants need to know.
6. Recommend a commit message.

Bootstrap Mode should be recorded as a decision when it becomes part of the standard workflow.

---

# Documentation Update Rules

Update documentation when:

- Project purpose changes
- Repo structure changes
- A new workflow is adopted
- Bootstrap Mode is enabled or revised
- A new prompt becomes reusable
- A significant decision is made
- A GitHub workflow is validated
- Deployment is added
- Another AI assistant contributes

Do not let important knowledge live only in chat.

---

# Security Rules

Never commit sensitive information.

For personal AI workflow projects, prefer private repositories unless there is a clear reason to make the repo public.

If environment variables are needed later, create `.env.example` only. Do not create or commit a real environment file.

---

# AI Agent Operating Instructions for GitHub Work

1. Read the project context.
2. Read the AI agent standard.
3. Read this GitHub setup template.
4. Check whether the GitHub repo exists.
5. If the repo exists, inspect existing files before modifying.
6. If the user asked to initialize, set up, standardize, or bootstrap the repo, enter Bootstrap Mode.
7. Create missing baseline files and folders when doing so does not overwrite existing work.
8. Preserve existing documentation.
9. Do not overwrite files unless instructed.
10. Update related documentation when appropriate.
11. Recommend a commit message.
12. Recommend issue or PR updates if relevant.
13. Update handoff notes after meaningful work.

---

# Default Recommendation for Mike's AI Workflow Validation Repo

```text
Repository name: ai-workflow-validation
GitHub owner: enderwillsaveyou
Visibility: private
Default branch: main
Initial mode: documentation-first
Purpose: Build, test, and refine reusable AI project standards, GitHub workflows, project context templates, prompt management, decision tracking, Bootstrap Mode, and multi-assistant collaboration.
```

The repo should begin as a documentation and workflow repository. Do not generate app code until the project moves beyond workflow validation.
