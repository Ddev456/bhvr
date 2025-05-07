# Plan d'implémentation Clean Architecture – BHVR

Documentation pour structurer le projet Carnet Potager avec la Clean Architecture, en partant de la base BHVR (Bun, Hono, Vite, React, Shadcn-ui) + RR7 (React Router v7 : https://remix.run/blog/merging-remix-and-react-router).

---

## 1. Étapes à suivre

### 1. Préparer la structure
- Créer le dossier `shared/core/` dans le monorepo BHVR
- Ajouter les sous-dossiers : `models/`, `usecases/`, `repositories/`, `__tests__/`

### 2. Déplacer la logique métier dans le core
- Types, modèles, règles métier, fonctions pures, use-cases → dans `shared/core/`
- L'UI (client) et l'API (server) consomment ce core

### 3. Utiliser le core dans le client et le serveur
- Importer les types et use-cases dans React et Hono
- L'UI ne fait que présenter les résultats et gérer les interactions

### 4. (Optionnel) Implémenter des mocks pour le développement
- Créer des implémentations "mock" des repositories pour tester l'UI sans backend

### 5. Tester le core
- Ajouter des tests unitaires dans `shared/core/__tests__/` pour valider la logique métier

---

## 2. Starter de structure de dossier

```
shared/
└── core/
    ├── types.ts
    ├── models/
    │   └── culture.ts
    ├── usecases/
    │   └── generateItinerary.ts
    ├── repositories/
    │   └── CultureRepository.ts
    └── __tests__/
        └── generateItinerary.test.ts
```

---

## 3. Exemple de use-case (TypeScript)

**shared/core/usecases/generateItinerary.ts**
```ts
import { Culture, Task } from '../types';

export function generateItinerary(culture: Culture): Task[] {
  // Logique métier pure ici
  return [
    { id: '1', label: 'Semis', date: '2025-03-01', status: 'todo' },
    { id: '2', label: 'Plantation', date: '2025-04-01', status: 'todo' },
    // ...
  ];
}
```

---

## 4. Template de test unitaire (Jest)

**shared/core/__tests__/generateItinerary.test.ts**
```ts
import { generateItinerary } from '../usecases/generateItinerary';
import { Culture } from '../types';

describe('generateItinerary', () => {
  it('génère un itinéraire de base pour une culture', () => {
    const culture: Culture = {
      id: 'c1',
      name: 'Tomate',
      zoneId: 'z1',
      tasks: []
    };
    const tasks = generateItinerary(culture);
    expect(tasks.length).toBeGreaterThan(0);
    expect(tasks[0].label).toBe('Semis');
  });
});
```

---

## 5. Pistes pour l'adaptation à BHVR
- Utiliser les alias TypeScript pour importer facilement le core dans client/server
- Documenter chaque use-case et modèle
- Commencer par les use-cases les plus critiques (ex : génération d'itinéraire, gestion des statuts de tâche)
- Garder le code du "core" pur (pas d'accès direct à l'UI, au réseau ou au stockage)

---

## 6. Ressources
- [Clean Architecture BHVR](./clean-architecture.md)
- [Repo BHVR](https://github.com/stevedylandev/bhvr)
- [Repo Angular Clean Architecture](https://github.com/eturlier/angular-clean-architecture) 