# Grasp AI

Utilise l'IA pour **comprendre**, **apprendre** et **maîtriser** plus vite toute chose (dont du code).

## Comment ça marche

1. Tu vois quelque chose que tu veux comprendre
2. Tu demandes à l'IA de te tester avec `/understand`
3. Tu expliques avec tes mots
4. L'IA détecte ce que tu maîtrises pas → crée une note
5. Tu révises avec `/revise_notes`

## Commandes

| Commande | Ce qu'elle fait |
|----------|-----------------|
| `/understand [code]` | L'IA te demande d'expliquer, note tes lacunes |
| `/revise_notes` | Révise tes notes jusqu'à maîtrise |

## Pourquoi ça marche

- **Active recall** : expliquer force à vraiment comprendre
- **Spaced repetition** : réviser au bon moment
- **Zettelkasten** : petites notes = meilleure rétention

## Quick start

```bash
git clone https://github.com/jblavisse/grasp-ai
cd grasp-ai

# Avec Claude Code
/understand [ton code]

# Avec Gemini CLI (gratuit)
/understand [ton code]

# Avec n'importe quelle IA
# → copie prompts/understand.md
```

## Apprendre le workflow IA

Les branches `level-0` à `level-5` t'apprennent à utiliser l'IA efficacement.

→ Voir `LEVEL-guide.md`
