# Comment apprendre avec ce système

## Le principe

Tu apprends en **expliquant**. Pas en lisant.

1. Tu regardes du code
2. Tu essaies d'expliquer
3. L'IA détecte tes lacunes
4. Une note est créée pour chaque concept flou
5. Tu révises plus tard

## 3 façons d'utiliser

### Option 1: Claude Code

```bash
/learn [ton code]
/review
```

Commandes dans `.claude/commands/`

### Option 2: Gemini CLI (gratuit)

```bash
/learn [ton code]
/review
```

Commandes dans `.gemini/commands/`

### Option 3: N'importe quelle IA (copier-coller)

1. Ouvre `prompts/learn.md` ou `prompts/review.md`
2. Copie le prompt
3. Colle dans ChatGPT, Gemini web, etc.
4. Crée/modifie les notes manuellement dans `notes/`

## Tes notes

Stockées dans `notes/` (gitignored = perso).

```markdown
---
status: todo
---

# Arrow Functions

Les arrow functions sont une syntaxe courte pour les fonctions.
Elles n'ont pas leur propre `this`.
```

## Le flow

```
/learn [code] → explique → note créée → /review → explique → note done
```

## Comparaison des outils

| Outil | Dossier | Gratuit |
|-------|---------|---------|
| Claude Code | `.claude/commands/` | Non |
| Gemini CLI | `.gemini/commands/` | ✅ Oui |
| Copier-coller | `prompts/` | ✅ Oui |

## Pourquoi ça marche

- **Active recall** : expliquer force à réfléchir
- **Spaced repetition** : réviser régulièrement
- **Zettelkasten** : petites notes atomiques
