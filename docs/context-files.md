# Context Files

How to give AI assistants context about your project.

## File names

| File | Tool | Purpose |
|------|------|---------|
| `CLAUDE.md` | Claude Code | Project instructions |
| `AGENTS.md` | Multiple | Generic agent config |
| `.cursorrules` | Cursor | Cursor-specific rules |
| `copilot-instructions.md` | Copilot | GitHub Copilot config |

## How it works

1. AI opens your project
2. AI reads the context file automatically
3. AI uses this context for all responses

## What to include

- Project description (1-2 sentences)
- Tech stack
- Folder structure
- Coding conventions
- Important decisions

## Tips

- Keep it short (AI has limited context)
- Update when project changes
- Use comments to explain sections
