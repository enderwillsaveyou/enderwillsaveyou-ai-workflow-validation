# Tool Compatibility

## ChatGPT Projects

- Upload the project instruction files into the project sources.
- Use GitHub connector access when repo updates are needed.
- Keep major decisions in repo files, not only in chat.

## Claude Projects

- Upload the same instruction files into the project folder.
- Ask Claude to inspect the repo or local folder before editing.
- Use the same Bootstrap Mode rules.

## Google Gemini / Gems

- Upload the same instruction files where supported.
- Use the project context file to ground each new chat.
- Keep reusable prompts in `prompts/`.

## GitHub Copilot

- Use `.github/copilot-instructions.md` for repo-specific guidance.
- Prefer documentation-first changes until code is needed.

## GitHub-Connected Coding Agents

- Inspect before editing.
- Avoid overwriting existing files.
- Update handoff notes after meaningful work.

## Local Coding Agents

- Treat the local folder as the working copy.
- Sync important changes back to GitHub.
- Recommend commits after meaningful updates.

## Future AI Tools

- Follow the same source-of-truth model.
- Preserve documentation and project history.
