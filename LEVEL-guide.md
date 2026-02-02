# Comment apprendre avec ce système

## Le principe

Tu apprends en **expliquant**. Pas en lisant.

1. Tu regardes du code
2. Tu essaies d'expliquer
3. L'IA détecte tes lacunes
4. Une note est créée pour chaque concept flou
5. Tu révises plus tard

## Commandes

### /learn [code]

```bash
/learn const add = (a, b) => a + b
```

L'IA te demande d'expliquer. Si t'expliques mal → note créée dans `notes/`.

### /review

```bash
/review
```

L'IA te fait réviser tes notes. Si t'expliques bien → note marquée `done`.

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

## Pourquoi ça marche

- **Active recall** : expliquer force à réfléchir
- **Spaced repetition** : réviser régulièrement
- **Zettelkasten** : petites notes atomiques

## À chaque level

1. Regarde le code/fichiers du level
2. Utilise `/learn` sur ce que tu comprends pas
3. Reviens plus tard avec `/review`
