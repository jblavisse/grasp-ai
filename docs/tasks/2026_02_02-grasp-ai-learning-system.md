# Instruction: grasp-ai Learning System

## Feature

- **Summary**: Progressive learning system teaching AI-assisted development through branched Git levels, from naive chat to automated skills with zettelkasten notes
- **Stack**: `Markdown`, `Claude Code CLI`, `Git`, `Bash`
- **Branch name**: `level-0` → `level-1` → `level-2` → `level-3` → `level-4` → `level-5`

## Existing files

- @CLAUDE.md
- @AGENTS.md
- @.gitignore

### New files to create

- `notes/` (gitignored)
- `prompts/explain.md`
- `prompts/commit.md`
- `prompts/pr.md`
- `.claude/commands/explain.md`
- `.claude/commands/commit.md`
- `.claude/commands/pr.md`
- `.claude/settings.json`
- `docs/trust-but-verify.md`

## Implementation phases

### Phase 1 - Setup + level-0

> Base structure, naive approach demo

1. Update .gitignore (add notes/)
2. Create notes/ folder with .gitkeep
3. Create README.md explaining project goal
4. Add docs/trust-but-verify.md (2 lines)
5. Commit + push branch `level-0`

### Phase 2 - level-1: Prompts templates

> Reusable markdown prompts (tool-agnostic)

1. Create prompts/explain.md (explain code template)
2. Create prompts/commit.md (commit message template)
3. Create prompts/pr.md (PR description template)
4. Add section on prompt iteration ("didn't work → rephrase")
5. Commit + push branch `level-1`

### Phase 3 - level-2: CLAUDE.md context

> Teach context injection via project files

1. Clean up CLAUDE.md with clear sections
2. Add learner-friendly comments explaining each section
3. Document how context files work (CLAUDE.md, AGENTS.md)
4. Commit + push branch `level-2`

### Phase 4 - level-3: Commands + commit/PR

> First automation with custom commands

1. Create .claude/commands/explain.md
2. Create .claude/commands/commit.md
3. Create .claude/commands/pr.md
4. Document command syntax and usage
5. Commit + push branch `level-3`

### Phase 5 - level-4: /explain skill + notes

> Smart skill that generates zettelkasten notes

1. Create skill /explain that:
   - Takes code input
   - Asks user to explain
   - Detects weak explanations
   - Creates minimal note in notes/
2. Note format: frontmatter (status: todo) + concept + 2-3 lines
3. Commit + push branch `level-4`

### Phase 6 - level-5: /review skill

> Spaced repetition review system

1. Create skill /review that:
   - Lists notes with status: todo
   - Presents concept to review
   - Updates status after review (todo → done)
2. Commit + push branch `level-5`

## Reviewed implementation

- [ ] Phase 1 - Setup + level-0
- [ ] Phase 2 - level-1: Prompts templates
- [ ] Phase 3 - level-2: CLAUDE.md context
- [ ] Phase 4 - level-3: Commands + commit/PR
- [ ] Phase 5 - level-4: /explain skill + notes
- [ ] Phase 6 - level-5: /review skill

## Validation flow

1. Clone repo fresh
2. Checkout each branch sequentially
3. Verify each level works independently
4. Test /explain with sample code → note created
5. Test /review → note reviewed and marked done
6. Verify prompts work with Gemini CLI (tool-agnostic)

## Estimations

- **Confidence**: 9/10
  - ✅ Clear scope, simple structure
  - ✅ Each phase is independent and testable
  - ✅ Zettelkasten format is minimal
  - ❌ Minor risk: skill syntax may need adjustment
- **Time to implement**: ~2-3 hours for all phases
