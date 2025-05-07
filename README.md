# Carnet Potager 🌱

> **MVP Kickoff**
>
> - **Vision** : Rendre le jardinage accessible à tous, avec un assistant interactif qui génère des itinéraires de culture personnalisés, sur une interface mobile-first.
> - **Objectif MVP** : Permettre à un débutant de créer un compte, configurer son profil, générer un itinéraire de culture pour une plante, et suivre ses tâches sur une timeline simple.
> - **Non-objectifs** : Pas de plan du jardin interactif, pas de notifications push, pas de partage entre utilisateurs, pas de cartographie avancée.
> - **Indicateurs de succès** : Nombre d'utilisateurs inscrits, nombre d'itinéraires générés, taux de complétion de l'onboarding, taux de retour/seconde visite.

---

## 🚀 Roadmap MVP (mai 2025)

| Semaine | Objectif principal | Jalons clés |
|---------|-------------------|-------------|
| Semaine 1 (6-12 mai) | Prototype interactif | Onboarding, assistant, génération d'un itinéraire, timeline simple |
| Semaine 2 | MVP complet | Carnet de culture, dashboard, gestion zones, tests UX |
| Semaine 3 | Améliorations | Finitions UI, accessibilité, responsive, corrections bugs |
| Semaine 4 | Préparation démo | Documentation, schémas, wireframes, bilan |

---

## ✅ Checklist d'avancement

- [ ] Onboarding utilisateur (création compte, configuration profil)
- [ ] Assistant interactif (questionnaire, génération itinéraire)
- [ ] Gestion des zones de culture (création, édition, suppression)
- [ ] Carnet de culture (fiche technique, carnet de bord, timeline)
- [ ] Timeline interactive (visualisation, validation tâches)
- [ ] Dashboard synthétique (vue d'ensemble, accès rapide)
- [ ] Responsive/mobile-first
- [ ] Tests UX (parcours débutant)
- [ ] Documentation technique et produit
- [ ] Wireframes et schémas (voir docs/wireframes.md et /docs/assets/)

---

## Présentation rapide

- **Assistant interactif** : Génère des itinéraires de culture personnalisés selon le climat, la saison, l'expérience et la disponibilité de l'utilisateur.
- **Gestion des zones de culture** : Créez et gérez jusqu'à 5 zones différentes (pleine terre, bac, serre, etc.) avec caractéristiques personnalisées.
- **Carnet de culture complet** : Fiches techniques générées, carnet de bord (notes, photos, réussites/échecs) et timeline interactive pour chaque culture.
- **Timeline interactive** : Visualisez et gérez toutes les tâches de jardinage sur une frise temporelle optimisée selon la région et la saison.
- **Dashboard synthétique** : Vue d'ensemble de toutes les cultures, tâches à venir, statistiques et accès rapide à l'assistant.

---

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

---

## 📎 Annexes

- [Wireframes textuels](docs/wireframes.md)
- Schémas et illustrations : `/docs/assets/`
