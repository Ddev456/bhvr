# Carnet Potager 🌱

Carnet Potager est une plateforme web pensée pour accompagner les jardiniers débutants et amateurs dans la gestion et le suivi de leur potager. L'objectif : rendre le jardinage simple, accessible et progressif grâce à une interface mobile-first et un assistant interactif.

## Présentation rapide

- **Assistant interactif** : Génère des itinéraires de culture personnalisés selon le climat, la saison, l'expérience et la disponibilité de l'utilisateur.
- **Gestion des zones de culture** : Créez et gérez jusqu'à 5 zones différentes (pleine terre, bac, serre, etc.) avec caractéristiques personnalisées.
- **Carnet de culture complet** : Fiches techniques générées, carnet de bord (notes, photos, réussites/échecs) et timeline interactive pour chaque culture.
- **Timeline interactive** : Visualisez et gérez toutes les tâches de jardinage sur une frise temporelle optimisée selon la région et la saison.
- **Dashboard synthétique** : Vue d'ensemble de toutes les cultures, tâches à venir, statistiques et accès rapide à l'assistant.

## Vision et objectifs

- Rendre le potager accessible à tous, notamment aux débutants.
- Proposer un outil simple, ergonomique et mobile-first.
- Accompagner l'apprentissage progressif et la planification saisonnière.

## Limites du MVP

- Maximum 10 itinéraires de culture par utilisateur
- Maximum 5 zones de culture
- Pas de notifications push ni de cartographie avancée
- Pas de partage entre utilisateurs

## Stack technique

- **Full-Stack TypeScript** : Type safety de bout en bout (client, serveur, types partagés)
- **Monorepo** : Organisation modulaire (client, serveur, shared)
- **Bun** pour le runtime JS, **Hono** pour l'API backend, **Vite** pour le frontend, **React** pour l'UI

## Structure du projet

```
.
├── client/    # Frontend React et React Router V7
├── server/    # Backend Hono
├── shared/    # Typescript partagé (types, modèles)
└── package.json
```
