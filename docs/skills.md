# Skills

Les skills sont des commandes avancées avec une logique multi-étapes.

## Skills disponibles

### /understand

Apprentissage interactif par l'explication de code.

```bash
/understand [colle ton code ici]
```

**Comment ça marche:**
1. Tu colles du code
2. L'IA te demande de l'expliquer
3. Tu expliques avec tes mots
4. L'IA identifie tes lacunes
5. L'IA crée des notes pour les concepts à revoir

**Exemple:**
```
> /understand const add = (a, b) => a + b

IA: Explique ce code avec tes mots.

Toi: C'est une fonction qui additionne deux nombres.

IA: Bien! Tu as compris le but.
    J'ai remarqué que tu n'as pas mentionné:
    - La syntaxe arrow function
    - Le return implicite

    Notes créées:
    - notes/arrow-functions.md
    - notes/return-implicite.md
```

## Format des notes

Les notes sont créées dans `notes/` (gitignored):

```markdown
---
status: todo
---

# Arrow Functions

Les arrow functions sont une syntaxe courte pour les fonctions.
Elles n'ont pas leur propre binding `this`.
```

### /revise_notes

Révise tes notes avec la répétition espacée.

```bash
/revise_notes
```

**Comment ça marche:**
1. L'IA liste les notes avec `status: todo`
2. Pour chaque note, l'IA te demande d'expliquer le concept
3. Si t'expliques bien → status passe à `done`
4. Si tu galères → reste `todo` pour la prochaine révision

**Exemple:**
```
> /revise_notes

IA: Révisons tes notes.
    Tu as 2 concepts à revoir.

    1/2: Explique "Arrow Functions" avec tes mots.

Toi: C'est une syntaxe courte avec () => {}

IA: Bien! Je marque comme done.

    2/2: Explique "Closures" avec tes mots.

Toi: Euh... un truc avec le scope?

IA: Pas tout à fait. Indice: c'est quand une fonction
    se souvient de son environnement.
    On reverra ça la prochaine fois.

    Résumé:
    - Révisées: 2
    - Maîtrisées: 1
    - À revoir: 1
```

## Pourquoi ça marche

- **Active recall**: expliquer force à réfléchir
- **Spaced repetition**: réviser régulièrement
- **Zettelkasten**: petites notes atomiques = meilleure rétention
