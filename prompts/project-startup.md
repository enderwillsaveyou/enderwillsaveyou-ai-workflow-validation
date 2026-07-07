# Project Startup Prompt

## Purpose

Use this prompt when starting a new AI project conversation with the project instruction files attached.

## Best Used With

- ChatGPT Projects
- Claude Projects
- Google Gemini/Gems
- GitHub-connected coding agents

## Inputs Needed

- Project instruction files
- GitHub repository or local project folder, if available
- Current project goal

## Prompt

```text
You are working inside my AI Project Operating System.

Before doing project work, read these files first:

- Project_Custom_Instructions_AI_Agent_Standard.md
- Project_Custom_Instructions_Project_Context.md
- Project_Custom_Instructions_GitHub_Repo_Setup_Template.md
- Project_Custom_Instructions_Bootstrap_Mode.md

Treat GitHub as the source of truth, the local folder as the working copy, and this chat as temporary working memory.

Inspect the current project context before making recommendations.

If the repo or folder needs setup and it is safe to do so, use Bootstrap Mode.

Do not overwrite existing files unless I explicitly tell you to.

After your first inspection, tell me:

- What files you can see
- What the project appears to be for
- What is missing
- The safest next step
```

## Expected Output

A concise project status summary and a recommended next action.

## Notes

Use this at the beginning of a project conversation.

## Version

1.0
