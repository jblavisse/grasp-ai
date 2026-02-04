# AGENTS.md

> This file gives context to AI assistants about your project.
> It works with Claude Code, Cursor, Copilot, and others.

<!--
HOW IT WORKS:
- AI reads this file automatically when you open the project
- Everything here becomes "context" for the AI
- More context = better answers
-->

## What is this project?

<!-- EDIT THIS: Describe your project in 1-2 sentences -->
A learning tool for AI-assisted development.

## Tech stack

<!-- EDIT THIS: List your main technologies -->
- Markdown
- Git
- Claude Code CLI (or any AI assistant)

## Rules for the AI

<!-- These rules tell the AI how to behave -->

### Be simple
- No over-engineering
- No extra features
- Focus on what's asked

### Be clear
- Short answers
- Bullet points
- Code examples when useful

### Be honest
- Say "I don't know" when unsure
- Ask for clarification if needed
- Challenge wrong assumptions

## Project structure

<!-- EDIT THIS: Describe your folder structure -->
```
prompts/     # Reusable prompt templates
notes/       # Personal learning notes (gitignored)
docs/        # Documentation
```

## Memory bank

<!--
Use this section to store important decisions and context.
The AI will remember this across conversations.
-->

### Decisions

- Using zettelkasten-style notes for learning
- Keeping prompts tool-agnostic (works with any AI)
