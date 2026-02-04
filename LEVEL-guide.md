# Apprendre à utiliser l'IA efficacement

Ce repo utilise des branches pour t'apprendre progressivement à booster ton workflow avec l'IA.

Checkout chaque level, explore les fichiers, et utilise `/understand` sur ce que tu vois.

---

## Level 0 - Chat basique

**Quoi:** Utiliser l'IA sans setup, juste copier-coller.

**Pourquoi:** C'est le point de départ. Tout le monde peut le faire.

**Comment:** Copie du code dans ChatGPT/Gemini et demande une explication.

**Ce qu'on attend:** Tu sais poser une question à une IA.

```bash
git checkout level-0
```

---

## Level 1 - Prompts templates

**Quoi:** Des prompts réutilisables dans `prompts/`.

**Pourquoi:** Écrire un bon prompt à chaque fois = perte de temps. Un template = consistance.

**Comment:** Ouvre `prompts/explain.md`, copie, colle avec ton code.

**Ce qu'on attend:** Tu as des prompts prêts à l'emploi.

```bash
git checkout level-1
```

---

## Level 2 - Contexte projet

**Quoi:** Fichiers `CLAUDE.md` / `GEMINI.md` / `AGENTS.md`.

**Pourquoi:** L'IA oublie tout entre chaque conversation. Ces fichiers lui donnent le contexte de ton projet automatiquement.

**Comment:** Regarde `AGENTS.md`, personnalise-le pour ton projet.

**Ce qu'on attend:** L'IA connaît ton projet sans que tu répètes.

```bash
git checkout level-2
```

---

## Level 3 - Commandes custom

**Quoi:** Commandes `/explain`, `/commit`, `/pr` dans `.claude/commands/` et `.gemini/commands/`.

**Pourquoi:** Taper le même prompt = répétitif. Une commande = un raccourci.

**Comment:** Tape `/explain [code]` au lieu de copier-coller un prompt.

**Ce qu'on attend:** Tu automatises tes interactions fréquentes.

```bash
git checkout level-3
```

---

## Level 4 - /understand + notes

**Quoi:** La commande `/understand` qui crée des notes pour tes lacunes.

**Pourquoi:** Lire une explication ≠ comprendre. Expliquer = vraie compréhension.

**Comment:** `/understand [code]` → explique → l'IA note ce que tu maîtrises pas.

**Ce qu'on attend:** Tu apprends activement, pas passivement.

```bash
git checkout level-4
```

---

## Level 5 - /revise_notes

**Quoi:** La commande `/revise_notes` pour réviser tes notes.

**Pourquoi:** On oublie 80% en 24h sans révision. Spaced repetition = rétention long terme.

**Comment:** `/revise_notes` → explique chaque concept → note marquée "done" si maîtrisé.

**Ce qu'on attend:** Tu maîtrises vraiment, pas juste "vu une fois".

```bash
git checkout level-5
```

---

## Résumé

| Level | Tu apprends | Fichiers clés |
|-------|-------------|---------------|
| 0 | Chat basique | - |
| 1 | Prompts templates | `prompts/` |
| 2 | Contexte projet | `AGENTS.md` |
| 3 | Commandes custom | `.claude/commands/`, `.gemini/commands/` |
| 4 | Apprentissage actif | `/understand` |
| 5 | Révision espacée | `/revise_notes` |

## Quel outil utiliser

| Outil | Dossier | Gratuit |
|-------|---------|---------|
| Claude Code | `.claude/commands/` | Non |
| Gemini CLI | `.gemini/commands/` | ✅ Oui |
| Copier-coller | `prompts/` | ✅ Oui |
