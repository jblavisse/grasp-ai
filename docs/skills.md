# Skills

Skills are advanced commands with multi-step logic.

## Available skills

### /understand

Interactive learning through code explanation.

```bash
/understand [paste code here]
```

**How it works:**
1. You paste code
2. AI asks you to explain it
3. You explain in your own words
4. AI identifies gaps in your understanding
5. AI creates notes for concepts you need to review

**Example session:**
```
> /understand const add = (a, b) => a + b

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

### /revise_notes

Review your notes with spaced repetition.

```bash
/revise_notes
```

**How it works:**
1. AI lists notes with `status: todo`
2. For each note, AI asks you to explain the concept
3. If you explain well → status changes to `done`
4. If you struggle → stays `todo` for next review

**Example session:**
```
> /revise_notes

AI: Let's review your notes.
    You have 2 concepts to review.

    1/2: Explain "Arrow Functions" in your own words.

You: They're shorter function syntax with () => {}

AI: Good! I've marked this as done.

    2/2: Explain "Closures" in your own words.

You: Uh... something with scope?

AI: Not quite. Hint: it's about functions
    remembering their environment.
    We'll review this again next time.

    Summary:
    - Reviewed: 2
    - Mastered: 1
    - Retry: 1
```

## Why this works

- **Active recall**: explaining forces you to think
- **Spaced repetition**: review notes regularly
- **Zettelkasten**: small atomic notes build knowledge
