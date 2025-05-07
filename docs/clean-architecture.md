# Clean Architecture dans BHVR (Bun, Hono, Vite, React) + Shadcn-UI & RR7

## Pourquoi Clean Architecture ?
La Clean Architecture vise à séparer la logique métier (core/domain) de l'UI (React) et de l'infrastructure (API, base de données). Cela permet :
- De tester la logique métier indépendamment de l'UI ou du backend
- De faire évoluer l'UI ou l'API sans toucher au métier
- De garder un code clair, maintenable, évolutif

## Structure recommandée pour BHVR

```
bhvr/
├── client/         # UI React (pages, composants, hooks, providers)
├── server/         # API Hono (routes, contrôleurs, services)
├── shared/
│   ├── core/       # Logique métier, types, use-cases, règles, modèles
│   └── ...         # Types partagés, utilitaires
└── ...
```

- **client/** : tout ce qui touche à l'affichage, la navigation, l'état local, l'intégration UI (Shadcn-ui, React Router v7...)
- **server/** : API REST, accès aux données, logique serveur
- **shared/core/** :
  - Types et modèles métier (Culture, Zone, Tâche, etc.)
  - Fonctions pures (génération d'itinéraires, calculs de dates, validation, etc.)
  - Use-cases (ex : `generateItinerary`, `addNoteToCulture`, etc.)
  - Interfaces (contrats) pour l'accès aux données (ex : `CultureRepository`)

## Dossier shared BHVR (Bun Hono Vite React) + shadcn-ui & React Router V7 (anciennement Remix) ?
- Le dossier `shared/` de BHVR est prévu pour partager des types et du code utilitaire entre client et serveur.
- **Pour la Clean Architecture** : Sous-dossier `core/` ou `domain/` dans `shared/` pour y placer toute la logique métier, les use-cases, les modèles, etc.
- **Exemple** :
  - `shared/core/types.ts` : types métier
  - `shared/core/usecases/` : fonctions métier
  - `shared/core/models/` : modèles
  - `shared/core/repositories/` : interfaces d'accès aux données

## Objectifs en tant que développeur web/ React junior
- Commencer simple : séparer la logique métier dans `shared/core/`, garder l'UI et l'API "minces"
- Tester la logique métier dans le core, sans dépendre de l'UI ou du backend
- Documenter la structure et les conventions
- Faire évoluer l'architecture en fonction de si le projet grossit ou devient collaboratif

## Ressources & sources inspirations
- [Repo BHVR](https://github.com/stevedylandev/bhvr)
- [Repo Angular Clean Architecture (exemple complet "avec Angular")](https://github.com/eturlier/angular-clean-architecture) 