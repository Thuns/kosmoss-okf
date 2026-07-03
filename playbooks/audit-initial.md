---
type: reference
title: Spécification officielle OKF v0.1
description: Référence vers la spécification officielle de l'Open Knowledge Format, publiée par Google Cloud le 12 juin 2026 sur GitHub.
tags: [okf, spec, google-cloud, référence, v0.1]
resource: https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md
created: 2026-07-02
updated: 2026-07-02
---

# Spécification officielle OKF v0.1

## Source

**Annoncé par** : Sam McVeety et Amir Hormati, Tech Leads, Data Analytics Engineering, Google Cloud  
**Date d'annonce** : 12 juin 2026  
**Licence** : Apache 2.0  
**Dépôt officiel** : [GoogleCloudPlatform/knowledge-catalog](https://github.com/GoogleCloudPlatform/knowledge-catalog)  
**Spec complète** : [okf/SPEC.md](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md)

## Points clés de la spec v0.1

- **Seul champ obligatoire** : `type` dans le frontmatter YAML
- **Noms de fichiers réservés** : `index.md` (sommaire) et `log.md` (historique)
- **Structure** : un répertoire de fichiers `.md`, organisé librement
- **Liens** : liens Markdown standards entre concepts (forment un graphe)
- **Versioning** : recommandé via Git

## Champs YAML recommandés (non obligatoires)

```yaml
type: concept        # ou: index, reference, playbook, runbook
title: Titre
description: Résumé en une phrase
tags: [tag1, tag2]
resource: https://url-de-reference.com
created: YYYY-MM-DD
updated: YYYY-MM-DD
```

## Ressources associées

- [FAQ OKF](https://okf.md/faq/)
- [Awesome OKF — liste de ressources communautaires](https://github.com/linyiru/awesome-okf)
- [Article d'annonce Google Cloud](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing)
- [LLM Wiki — Andrej Karpathy (inspiration originale)](https://gist.github.com/karpathy/llm-wiki)

## Liens connexes

- [Open Knowledge Format (OKF) — concept](../concepts/okf.md)
- [Le Catalogue de Connaissance — service Kosmoss](../services/catalogue-connaissance.md)
