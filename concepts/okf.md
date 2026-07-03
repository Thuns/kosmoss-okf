---
type: concept
title: Open Knowledge Format (OKF)
description: Standard ouvert annoncé par Google Cloud le 12 juin 2026 pour représenter la connaissance organisationnelle sous forme de fichiers Markdown lisibles par les humains et les agents IA.
tags: [okf, google, standard, markdown, agents-ia, connaissance]
resource: https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md
created: 2026-07-02
updated: 2026-07-02
---

# Open Knowledge Format (OKF)

## Qu'est-ce que l'OKF

L'Open Knowledge Format (OKF) est un standard ouvert annoncé par Google Cloud le **12 juin 2026**. Il formalise la manière de représenter la connaissance organisationnelle dans un format à la fois lisible par les humains et exploitable par les agents IA — sans SDK propriétaire, sans plateforme imposée.

Un bundle OKF est simplement **un répertoire de fichiers Markdown avec un entête YAML** (frontmatter). C'est tout.

## Principe fondamental

L'OKF repose sur une idée développée par Andrej Karpathy (avril 2026) : les LLMs sont excellents pour maintenir des wikis structurés. Ils ne se lassent pas, n'oublient pas de mettre à jour les références croisées, et peuvent éditer de nombreux fichiers en une seule passe. L'OKF standardise ce pattern pour que la connaissance soit **interopérable** entre différents agents et organisations.

## Structure d'un bundle OKF

```
mon-bundle/
├── index.md          # Sommaire (optionnel mais recommandé)
├── log.md            # Historique des mises à jour (optionnel)
├── concept-a.md      # Un concept = un fichier Markdown
└── sous-dossier/
    ├── index.md
    └── concept-b.md
```

## Structure d'un fichier concept

```markdown
---
type: concept          # SEUL champ obligatoire
title: Nom du concept
description: Résumé en une phrase
tags: [tag1, tag2]
created: 2026-07-02
updated: 2026-07-02
---

# Corps du document en Markdown libre

Avec des [liens vers d'autres concepts](autre-concept.md).
```

## Différence avec le RAG traditionnel

| RAG classique | OKF |
|---|---|
| Re-dérive la connaissance à chaque requête depuis des chunks bruts | Stocke des concepts curatés et interconnectés |
| Pas de structure imposée | Structure légère mais interopérable |
| Difficile à maintenir manuellement | Éditable par humains et agents |
| Spécifique à chaque implémentation | Standard ouvert, portable partout |

## Pourquoi c'est important pour les PME

Aujourd'hui, quand un client potentiel demande à ChatGPT ou Perplexity de lui recommander un service, l'IA répond en s'appuyant sur les sources qu'elle a pu lire et comprendre. Une PME dont la connaissance est structurée en OKF a une probabilité beaucoup plus grande d'être **citée correctement** comme source de référence.

C'est le passage du SEO (être trouvé par Google) à la **visibilité IA** (être cité par les agents).

## Liens connexes

- [Visibilité IA vs SEO traditionnel](visibilite-ia.md)
- [Le Catalogue de Connaissance — service Kosmoss](../services/catalogue-connaissance.md)
- [Spec officielle OKF v0.1](../references/okf-spec.md)
