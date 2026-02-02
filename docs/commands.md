# Custom Commands

Commands let you run prompts with a shortcut.

## Usage (Claude Code)

```bash
/explain [paste code here]
/commit
/pr
```

## How it works

1. Commands live in `.claude/commands/`
2. Each `.md` file = one command
3. File name = command name
4. `$ARGUMENTS` = what you type after the command

## Example

File: `.claude/commands/explain.md`
```markdown
Explain this code:
$ARGUMENTS
```

Usage:
```
/explain function add(a, b) { return a + b }
```

## Available commands

| Command | What it does |
|---------|--------------|
| `/explain` | Explain code step by step |
| `/commit` | Generate commit message |
| `/pr` | Generate PR description |
