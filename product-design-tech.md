# Analyse Produit / Tech & Design – Carnet Potager 🌱

> **Ce document synthétise les choix structurants pour le MVP, avec un focus sur l'alignement produit, technique et design. Les décisions clés sont encadrées et chaque section est reliée à la vision et au scope MVP.**

---

## 1. Aspect Produit

### 1.1 Proposition de valeur
- **Mission principale** : Rendre le jardinage/potager facile pour tout le monde, même sans expérience.
- **Promesse utilisateur** : Simplifier via une interface ergonomique la découverte/gestion du potager.
- **Différenciation** : Assistant interactif générant des itinéraires personnalisés.

> **Décision MVP** : L'assistant interactif est la fonctionnalité cœur du MVP ([voir vision-goals.md](vision-goals.md)).

### 1.2 Segmentation utilisateurs
- **Cible principale** : Jardiniers débutants et amateurs
- **Personas** : Julie (débutante, mobile), Marc (amateur, suivi avancé)

### 1.3 Fonctionnalités clés (MVP)
- Assistant interactif (questionnaire, génération d'itinéraires)
- Gestion des zones de culture (max 5)
- Carnet de culture (fiche technique, carnet de bord, timeline)
- Dashboard synthétique

> **Décision MVP** : Limiter à 10 itinéraires et 5 zones, pas de fonctionnalités avancées hors MVP ([voir README.md](../README.md))

### 1.4 Modèle économique
- **Freemium** envisagé, mais non prioritaire pour le MVP

> **Décision MVP** : Pas de paywall, focus sur l'expérience gratuite et complète pour valider l'usage.

### 1.5 Croissance et engagement
- Acquisition : SEO, contenu éducatif, partenariats
- Activation/rétention : Onboarding guidé, gamification, emails/newsletter

### 1.6 Roadmap d'évolution
- **Phase 1 (MVP)** : Assistant, carnet, dashboard, gestion zones
- **Phase 2** : Communauté, partage, notifications
- **Phase 3** : Plan du jardin interactif, fonctionnalités avancées

> **Décision** : La roadmap MVP est détaillée dans le [README.md](../README.md) (section Roadmap).

### 1.7 Métriques de succès
- Nombre d'utilisateurs inscrits/actifs
- Nombre d'itinéraires générés
- Taux de complétion onboarding
- Taux de retour/seconde visite

---

## 2. Aspect Tech

### 2.1 Choix du framework frontend
- **Décision MVP** : React + React Router V7 ([voir README.md](../README.md)), pour rapidité, écosystème, et compatibilité mobile-first.

### 2.2 Architecture technique
- **Frontend** : Architecture par composants réutilisables, design system, gestion d'état simple (useState/useContext ou Jotai/MobX si besoin)
- **Backend** : API RESTful (Hono), types partagés (shared/)
- **Base de données** : PostgreSQL (par défaut)

> **Décision** : Architecture modulaire monorepo (client/server/shared)

### 2.3 Infrastructure cloud
- **Frontend** : Netlify (prototype), autres options à explorer
- **Backend** : Coolify ou équivalent
- **CI/CD** : Simple (GitHub Actions si besoin)

### 2.4 Optimisation technique
- **Mobile-first** : Priorité absolue
- **Performance** : Lazy loading, cache, optimisation images

### 2.5 Intégrations techniques
- APIs tierces (météo, base plantes, géoloc)
- Services (notifications, emails, paiement) hors MVP

### 2.6 Sécurité et conformité
- RGPD, authentification simple, sauvegarde régulière

---

## 3. Aspect Design (Conception)

### 3.1 Recherche et découverte
- Entretiens utilisateurs, benchmark, analyse marché

### 3.2 Stratégie UX
- Simplicité, contextualisation, progression visible, autonomisation
- Architecture de l'information intuitive

### 3.3 Conception d'interaction
- Wireframes textuels ([voir docs/wireframes.md](docs/wireframes.md))
- Prototypes à réaliser avec Penpot ([voir /docs/assets/](../docs/assets/))

### 3.4 Design System
- Palette nature, typographie lisible, iconographie cohérente
- Composants UI réutilisables, accessibilité (WCAG)

### 3.5 Validation et itération
- Tests utilisateurs, cycles courts, amélioration continue

---

## 4. Synergie produit/tech/design
- Les choix techniques servent la vision produit (assistant, simplicité, mobile-first)
- La conception UI/UX incarne la proposition de valeur (guidage, accessibilité)
- L'architecture modulaire facilite l'évolution future

---

> **Pour plus de détails, voir :**
> - [README.md](../README.md) (MVP Kickoff, roadmap, checklist)
> - [vision-goals.md](vision-goals.md) (vision, non-objectifs, indicateurs)
> - [features.md](features.md) (fonctionnalités détaillées)
> - [user-stories.md](user-stories.md) (user stories priorisées)
> - [docs/wireframes.md](docs/wireframes.md) (wireframes textuels)