# GitHub Workflow

## Source of Truth

GitHub is the permanent source of truth for this project.

The local project folder is the working copy.

AI chat conversations are temporary working memory.

## Branch Strategy

For this solo workflow validation repo, keep branching simple.

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

## Commit Strategy

Use small, descriptive commits.

Good examples:

```text
Initialize AI workflow validation repository
Add Bootstrap Mode instructions
Document decision tracking workflow
Add prompt management structure
Update project context
```

Avoid vague commit messages such as `updates`, `stuff`, `final`, or `misc`.

## Issue Workflow

Use issues to track reusable improvements, validation tasks, and future tests.

Recommended labels:

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

## Pull Request Expectations

Pull requests are optional for small personal documentation edits.

Use pull requests when:

- Testing AI-assisted GitHub workflows.
- Reviewing larger documentation changes.
- Changing the project standard.
- Adding reusable templates.
- Testing collaboration between multiple AI assistants.

## Documentation Update Rules

Update documentation when:

- Project purpose changes.
- Repo structure changes.
- A new workflow is adopted.
- Bootstrap Mode is enabled or revised.
- A new prompt becomes reusable.
- A significant decision is made.
- Another AI assistant contributes.

## Bootstrap Mode Behavior

When the user asks to initialize, set up, prepare, standardize, or bootstrap an existing repo or folder, the assistant should:

1. Inspect first.
2. Preserve existing files.
3. Create missing baseline documentation and workflow files.
4. Avoid overwriting non-placeholder files.
5. Update `agents/handoff.md`, `docs/decisions.md`, and `docs/changelog.md` when meaningful setup work is done.

## Local Folder vs GitHub

If both a GitHub repository and local folder are available, GitHub is the source of truth unless Mike says the local folder has newer work.
