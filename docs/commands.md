# Commandes custom

Les commandes te permettent de lancer des prompts avec un raccourci.

## Usage (Claude Code)

```bash
/explain [colle ton code ici]
/commit
/pr
```

## Comment ça marche

1. Les commandes sont dans `.claude/commands/`
2. Chaque fichier `.md` = une commande
3. Nom du fichier = nom de la commande
4. `$ARGUMENTS` = ce que tu tapes après la commande

## Exemple

Fichier: `.claude/commands/explain.md`
```markdown
Explique ce code:
$ARGUMENTS
```

Usage:
```
/explain function add(a, b) { return a + b }
```

## Commandes disponibles

| Commande | Ce qu'elle fait |
|----------|-----------------|
| `/explain` | Explique du code étape par étape |
| `/commit` | Génère un message de commit |
| `/pr` | Génère une description de PR |
| `/understand` | Teste ta compréhension + crée des notes |
| `/revise_notes` | Révise tes notes |
