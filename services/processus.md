---
type: concept
title: Processus de livraison — 4 phases sur 6 semaines
description: Processus structuré de construction d'un Catalogue de Connaissance OKF pour un client PME, de l'audit initial à la mise en ligne et à la maintenance mensuelle.
tags: [processus, livraison, phases, audit, okf, 6-semaines]
created: 2026-07-02
updated: 2026-07-02
---

# Processus de livraison — 4 phases

## Vue d'ensemble

La construction d'un Catalogue de Connaissance se déroule sur **6 semaines** pour le livrable initial, suivie d'une maintenance mensuelle continue.

---

## Phase 1 — Audit de connaissance (semaines 1-2)

**Objectif** : cartographier ce que l'entreprise sait vs. ce qui est structuré numériquement.

### Activités
- Entretiens avec 2-3 experts internes (1h chacun, en personne ou vidéo)
- Analyse de la présence IA actuelle : que dit ChatGPT, Perplexity, Gemini sur l'entreprise aujourd'hui ?
- Inventaire des documents existants (site web, brochures, politiques, processus)
- Identification des concepts prioritaires à structurer en premier

### Livrable
Rapport d'audit (document PDF) + liste priorisée des concepts à documenter

---

## Phase 2 — Construction du bundle OKF (semaines 3-5)

**Objectif** : créer les fichiers Markdown conformes OKF v0.1 pour chaque concept prioritaire.

### Activités
- Rédaction des fichiers de concepts (services, zones, FAQ, tarifs, processus, expertises)
- Création des liens croisés entre concepts (le graphe de connaissance)
- Validation du contenu avec le client (une révision incluse)
- Création du fichier `index.md` (point d'entrée pour les agents IA)
- Création du fichier `log.md` (historique)

### Livrable
Bundle OKF complet, versionné sur GitHub + documentation d'utilisation

---

## Phase 3 — Activation IA (semaine 6)

**Objectif** : rendre le bundle lisible et indexable par les agents IA.

### Activités
- Dépôt du bundle dans le dossier `/okf/` du site web du client
- Création du fichier `llms.txt` à la racine du site
- Ajout des schémas JSON-LD (schema.org) sur les pages clés du site WordPress
- Test de visibilité : questions de test posées à ChatGPT, Perplexity, Gemini
- Rapport de visibilité "avant/après" (état initial vs. état au lancement)

### Livrable
Bundle en ligne + rapport de lancement avec captures d'écran des tests IA

---

## Phase 4 — Maintenance mensuelle (récurrent)

**Objectif** : garder le bundle vivant et exact à mesure que l'entreprise évolue.

### Activités mensuelles
- Mise à jour des concepts existants (nouveaux projets, changements de service, nouvelles FAQ)
- Ajout de nouveaux concepts si nécessaire
- Mise à jour du `log.md` avec l'historique des changements
- Rapport mensuel de citations IA : quand et comment les agents mentionnent l'entreprise
- Recommandations pour le mois suivant

### Pourquoi c'est récurrent par nature
Un bundle OKF n'est jamais "terminé". Chaque nouveau projet livré, chaque nouveau service, chaque changement de tarif ou de réglementation doit être reflété dans le bundle pour que l'IA continue de citer des informations exactes. C'est structurellement un service continu.

---

## Liens connexes

- [Le Catalogue de Connaissance](catalogue-connaissance.md)
- [Les paliers de service](paliers.md)
- [Playbook d'audit initial](../playbooks/audit-initial.md)
