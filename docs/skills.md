# Skills

Skills are advanced commands with multi-step logic.

## Available skills

### /learn

Interactive learning through code explanation.

```bash
/learn [paste code here]
```

**How it works:**
1. You paste code
2. AI asks you to explain it
3. You explain in your own words
4. AI identifies gaps in your understanding
5. AI creates notes for concepts you need to review

**Example session:**
```
> /learn const add = (a, b) => a + b

AI: Explain this code in your own words.

You: It's a function that adds two numbers.

AI: Good! You understood the basic purpose.
    I noticed you didn't mention:
    - Arrow function syntax
    - Implicit return

    Created notes:
    - notes/arrow-functions.md
    - notes/implicit-return.md
```

## Note format

Notes are created in `notes/` (gitignored):

```markdown
---
status: todo
---

# Arrow Functions

Arrow functions are a shorter syntax for functions.
They don't have their own `this` binding.
```

## Why this works

- **Active recall**: explaining forces you to think
- **Spaced repetition**: review notes later with /review
- **Zettelkasten**: small atomic notes build knowledge
