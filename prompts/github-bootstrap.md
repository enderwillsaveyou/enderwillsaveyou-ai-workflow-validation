# GitHub Bootstrap Prompt

## Purpose

Use this prompt when asking an AI assistant with GitHub access to inspect and bootstrap an existing repository.

## Best Used With

- ChatGPT with GitHub connector
- GitHub-connected coding agents
- GitHub Copilot-style repo workflows

## Inputs Needed

- Repository full name, such as `owner/repo-name`
- Project instruction files
- Any known project purpose or constraints

## Prompt

```text
You are working inside my AI Project Operating System.

Read these project instruction files first:

- Project_Custom_Instructions_AI_Agent_Standard.md
- Project_Custom_Instructions_Project_Context.md
- Project_Custom_Instructions_GitHub_Repo_Setup_Template.md
- Project_Custom_Instructions_Bootstrap_Mode.md

Inspect the GitHub repository before changing anything.

If the repository is missing the standard baseline structure, enter Bootstrap Mode and create the missing files and folders immediately when safe.

Do not overwrite existing files unless I explicitly tell you to.

If the repo is empty or only has a minimal README, initialize the documentation-first project structure from the templates.

Keep GitHub as the source of truth, the local folder as the working copy, and the chat as temporary working memory.

After setup, report:

- Files created
- Files preserved
- Files skipped
- Missing information
- Recommended next step
- Recommended commit message
```

## Expected Output

A repository setup summary with files created, preserved, skipped, and a recommended commit message.

## Notes

Use this only after the repository exists.

## Version

1.0
