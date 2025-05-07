# User stories principales – Carnet Potager 🌱

> Ce document décrit les user stories principales pour le MVP, avec critères d'acceptation, tags MVP, priorités explicites, et liens vers les fonctionnalités. Il sert de backlog priorisé pour le développement.

---

## Légende
- **[MVP]** : Inclus dans le MVP
- **Priorité** : HAUTE / MOYENNE / BASSE
- **Lien feature** : Voir [features.md](features.md)

---

### 👤 Types d'utilisateurs
- Débutant : Utilisateur novice en jardinage avec peu ou pas d'expérience
- Amateur : Utilisateur avec quelques bases et une certaine expérience de jardinage
- Tous : Applicable à tous les types d'utilisateurs

---

## 🔐 Compte utilisateur et configuration initiale

| ID    | En tant que... | Je veux... | Afin de... | Priorité | [MVP] | Critères d'acceptation |
|-------|----------------|------------|------------|----------|-------|-----------------------|
| US-01 | Tous           | M'inscrire avec mon email et un mot de passe | Créer mon compte personnel | HAUTE | ✅ | Donné un utilisateur non inscrit, Quand il renseigne un email et un mot de passe valides, Alors un compte est créé et il accède à l'onboarding |
| US-02 | Tous           | Me connecter à mon compte | Accéder à mes données personnelles | HAUTE | ✅ | Donné un compte existant, Quand je saisis mes identifiants, Alors je suis connecté et redirigé vers le dashboard |
| US-03 | Tous           | Configurer ma région/climat | Recevoir des recommandations adaptées | HAUTE | ✅ | Donné un utilisateur connecté, Quand il configure sa région, Alors les recommandations de l'assistant sont adaptées |
| US-04 | Tous           | Définir mon niveau d'expérience | Adapter l'interface et les conseils à mon expérience | HAUTE | ✅ | Donné un utilisateur connecté, Quand il choisit son niveau, Alors l'interface et les conseils sont adaptés |
| US-05 | Tous           | Indiquer mes jours de jardinage préférés | Organiser les tâches selon ma disponibilité | MOYENNE | ✅ | Donné un utilisateur connecté, Quand il sélectionne ses jours, Alors la planification des tâches en tient compte |
| US-06 | Tous           | Configurer ma zone de rusticité | Adapter les périodes de culture à mon climat | HAUTE | ✅ | Donné un utilisateur connecté, Quand il configure sa zone, Alors les périodes de culture sont adaptées |

---

## 🗂️ Gestion des zones de culture ([features.md](features.md) – Essentiel, MVP)

| ID    | En tant que... | Je veux... | Afin de... | Priorité | [MVP] | Critères d'acceptation |
|-------|----------------|------------|------------|----------|-------|-----------------------|
| US-10 | Tous           | Créer une nouvelle zone de culture | Définir un nouvel espace de jardinage | HAUTE | ✅ | Donné un utilisateur connecté, Quand il renseigne les infos d'une zone, Alors la zone est créée et listée |
| US-11 | Tous           | Spécifier le type de zone | Adapter les recommandations au type de contenant | HAUTE | ✅ | Donné une zone créée, Quand je choisis le type, Alors les conseils sont adaptés |
| US-12 | Tous           | Configurer l'exposition de ma zone | Recevoir des conseils adaptés à l'ensoleillement | HAUTE | ✅ | Donné une zone créée, Quand j'indique l'exposition, Alors les conseils sont adaptés |
| US-13 | Tous           | Définir les dimensions/surface de ma zone | Gérer mon espace de jardinage | MOYENNE | ✅ | Donné une zone créée, Quand je renseigne les dimensions, Alors elles sont enregistrées et affichées |
| US-14 | Tous           | Spécifier le type de sol | Adapter les recommandations aux conditions spécifiques | MOYENNE | ✅ | Donné une zone créée, Quand je choisis le type de sol, Alors les conseils sont adaptés |
| US-15 | Tous           | Modifier les paramètres d'une zone existante | Mettre à jour les informations | HAUTE | ✅ | Donné une zone existante, Quand je modifie ses paramètres, Alors ils sont mis à jour |
| US-16 | Tous           | Supprimer une zone de culture | Retirer les zones que je n'utilise plus | MOYENNE | ✅ | Donné une zone existante, Quand je la supprime, Alors elle disparaît de la liste |
| US-17 | Tous           | Nommer mes zones de façon personnalisée | Les identifier facilement | HAUTE | ✅ | Donné une zone créée, Quand je saisis un nom, Alors il est affiché partout dans l'UI |

---

## 🤖 Assistant interactif ([features.md](features.md) – Essentiel, MVP)

| ID    | En tant que... | Je veux... | Afin de... | Priorité | [MVP] | Critères d'acceptation |
|-------|----------------|------------|------------|----------|-------|-----------------------|
| US-20 | Tous           | Lancer l'assistant de création d'un nouvel itinéraire | Planifier une nouvelle culture | HAUTE | ✅ | Donné un utilisateur connecté, Quand il clique sur "Nouvelle culture", Alors l'assistant démarre |
| US-21 | Tous           | Sélectionner une zone pour ma nouvelle culture | Associer la culture à un espace spécifique | HAUTE | ✅ | Donné l'assistant lancé, Quand je sélectionne une zone, Alors elle est associée à la culture |
| US-22 | Tous           | Choisir une plante à cultiver | Démarrer la planification d'une culture précise | HAUTE | ✅ | Donné l'assistant lancé, Quand je choisis une plante, Alors elle est affichée dans le récapitulatif |
| US-23 | Tous           | Spécifier mon point de départ (semis, plants) | Adapter l'itinéraire selon ma méthode | HAUTE | ✅ | Donné l'assistant lancé, Quand je choisis le point de départ, Alors l'itinéraire s'adapte |
| US-24 | Tous           | Préciser une variété spécifique | Personnaliser ma culture | MOYENNE | ✅ | Donné l'assistant lancé, Quand je renseigne une variété, Alors elle est prise en compte |
| US-25 | Débutant       | Recevoir des instructions détaillées | Comprendre chaque étape du processus | HAUTE | ✅ | Donné l'assistant lancé, Quand je suis débutant, Alors les instructions sont détaillées |
| US-26 | Amateur        | Recevoir des instructions concises | Avancer plus rapidement dans le processus | MOYENNE | ✅ | Donné l'assistant lancé, Quand je suis amateur, Alors les instructions sont concises |
| US-27 | Tous           | Générer un itinéraire de culture complet | Obtenir un plan détaillé pour ma culture | HAUTE | ✅ | Donné l'assistant lancé, Quand j'ai répondu à toutes les questions, Alors un itinéraire est généré |
| US-28 | Tous           | Modifier l'itinéraire généré | Personnaliser les étapes selon mes besoins | HAUTE | ✅ | Donné un itinéraire généré, Quand je modifie une étape, Alors l'itinéraire est mis à jour |

---

## 📒 Carnet de culture ([features.md](features.md) – Essentiel, MVP)

| ID    | En tant que... | Je veux... | Afin de... | Priorité | [MVP] | Critères d'acceptation |
|-------|----------------|------------|------------|----------|-------|-----------------------|
### 🔐 Compte utilisateur et configuration initiale
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-01
			Tous
			M'inscrire avec mon email et un mot de passe
			Créer mon compte personnel
			HAUTE
			US-02
			Tous
			Me connecter à mon compte
			Accéder à mes données personnelles
			HAUTE
			US-03
			Tous
			Configurer ma région/climat
			Recevoir des recommandations adaptées
			HAUTE
			US-04
			Tous
			Définir mon niveau d'expérience (débutant/avancé)
			Adapter l'interface et les conseils à mon expérience
			HAUTE
			US-05
			Tous
			Indiquer mes jours de jardinage préférés
			Organiser les tâches selon ma disponibilité
			MOYENNE
			US-06
			Tous
			Configurer ma zone de rusticité
			Adapter les périodes de culture à mon climat
			HAUTE
### 🗂️ Gestion des zones de culture
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-10
			Tous
			Créer une nouvelle zone de culture
			Définir un nouvel espace de jardinage
			HAUTE
			US-11
			Tous
			Spécifier le type de zone (pleine terre, pot, bac, etc.)
			Adapter les recommandations au type de contenant
			HAUTE
			US-12
			Tous
			Configurer l'exposition de ma zone
			Recevoir des conseils adaptés à l'ensoleillement
			HAUTE
			US-13
			Tous
			Définir les dimensions/surface de ma zone
			Gérer mon espace de jardinage
			MOYENNE
			US-14
			Tous
			Spécifier le type de sol
			Adapter les recommandations aux conditions spécifiques
			MOYENNE
			US-15
			Tous
			Modifier les paramètres d'une zone existante
			Mettre à jour les informations
			HAUTE
			US-16
			Tous
			Supprimer une zone de culture
			Retirer les zones que je n'utilise plus
			MOYENNE
			US-17
			Tous
			Nommer mes zones de façon personnalisée
			Les identifier facilement
			HAUTE
### 🤖 Assistant interactif
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-20
			Tous
			Lancer l'assistant de création d'un nouvel itinéraire
			Planifier une nouvelle culture
			HAUTE
			US-21
			Tous
			Sélectionner une zone pour ma nouvelle culture
			Associer la culture à un espace spécifique
			HAUTE
			US-22
			Tous
			Choisir une plante à cultiver
			Démarrer la planification d'une culture précise
			HAUTE
			US-23
			Tous
			Spécifier mon point de départ (semis, plants)
			Adapter l'itinéraire selon ma méthode
			HAUTE
			US-24
			Tous
			Préciser une variété spécifique
			Personnaliser ma culture
			MOYENNE
			US-25
			Débutant
			Recevoir des instructions détaillées
			Comprendre chaque étape du processus
			HAUTE
			US-26
			Amateur
			Recevoir des instructions concises
			Avancer plus rapidement dans le processus
			MOYENNE
			US-27
			Tous
			Générer un itinéraire de culture complet
			Obtenir un plan détaillé pour ma culture
			HAUTE
			US-28
			Tous
			Modifier l'itinéraire généré
			Personnaliser les étapes selon mes besoins
			HAUTE
### 📒 Carnet de culture
#### Fiche technique
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-30
			Tous
			Consulter la fiche technique d'une plante
			Connaître ses caractéristiques et besoins
			HAUTE
			US-31
			Débutant
			Voir les erreurs communes à éviter
			Maximiser mes chances de réussite
			HAUTE
			US-32
			Tous
			Consulter les associations favorables/défavorables
			Optimiser mes associations de cultures
			MOYENNE
			US-33
			Tous
			Voir les maladies et ravageurs courants
			Identifier et prévenir les problèmes
			MOYENNE
			US-34
			Tous
			Accéder aux conseils de culture
			Améliorer mes techniques
			HAUTE
#### Carnet de bord
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-40
			Tous
			Ajouter une note de suivi
			Documenter l'évolution de ma culture
			HAUTE
			US-41
			Tous
			Ajouter une photo
			Illustrer visuellement ma culture
			HAUTE
			US-42
			Tous
			Enregistrer mes réussites
			Documenter ce qui a bien fonctionné
			MOYENNE
			US-43
			Tous
			Noter mes échecs
			Éviter de répéter les mêmes erreurs
			MOYENNE
			US-44
			Tous
			Catégoriser mes notes avec des tags
			Organiser et retrouver facilement mes observations
			BASSE
			US-45
			Tous
			Consulter l'historique chronologique de mes notes
			Suivre l'évolution dans le temps
			HAUTE
#### Itinéraire de culture
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-50
			Tous
			Visualiser mon itinéraire sur une timeline
			Avoir une vue d'ensemble de ma culture
			HAUTE
			US-51
			Tous
			Marquer une tâche comme réalisée
			Suivre ma progression
			HAUTE
			US-52
			Tous
			Marquer une tâche comme 'en cours'
			Indiquer ce sur quoi je travaille actuellement
			MOYENNE
			US-53
			Tous
			Modifier la date d'une tâche
			Adapter mon planning
			HAUTE
			US-54
			Tous
			Ajouter une nouvelle tâche
			Compléter mon itinéraire
			HAUTE
			US-55
			Tous
			Marquer une tâche comme 'ignorée'
			Sauter les étapes non pertinentes
			BASSE
			US-56
			Tous
			Voir la difficulté et durée estimée des tâches
			Mieux planifier mon temps
			MOYENNE
### ⏳ Timeline interactive
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-60
			Tous
			Scroller horizontalement dans ma timeline
			Naviguer dans le temps
			HAUTE
			US-61
			Tous
			Zoomer/dézoomer sur ma timeline
			Ajuster la granularité temporelle
			MOYENNE
			US-62
			Tous
			Voir les tâches par code couleur
			Identifier rapidement les types d'actions
			MOYENNE
			US-63
			Tous
			Centrer automatiquement sur la période actuelle
			Voir mes tâches immédiates
			HAUTE
			US-64
			Tous
			Déplacer des tâches par drag & drop
			Réorganiser mon planning
			HAUTE
			US-65
			Tous
			Accéder rapidement aux détails d'une tâche
			Consulter les instructions détaillées
			HAUTE
			US-66
			Tous
			Ajouter des notes/photos depuis la timeline
			Enrichir mon suivi
			MOYENNE
			US-67
			Tous
			Voir quelle zone est concernée par chaque tâche
			Organiser mon travail par espace
			MOYENNE
### 📊 Dashboard
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-70
			Tous
			Voir une synthèse de toutes mes cultures
			Avoir une vue d'ensemble de mon potager
			HAUTE
			US-71
			Tous
			Filtrer mes cultures par zone
			Me concentrer sur un espace spécifique
			HAUTE
			US-72
			Tous
			Trier mes cultures par différents critères
			Organiser mon affichage selon mes besoins
			MOYENNE
			US-73
			Tous
			Voir mes prochaines tâches
			Planifier mon temps de jardinage
			HAUTE
			US-74
			Tous
			Accéder directement à une culture
			Consulter rapidement une culture spécifique
			HAUTE
			US-75
			Tous
			Voir le nombre de tâches par statut
			Évaluer ma progression globale
			MOYENNE
			US-76
			Tous
			Créer une nouvelle culture
			Démarrer un nouvel itinéraire
			HAUTE
			US-77
			Tous
			Supprimer une culture
			Retirer les cultures terminées ou abandonnées
			MOYENNE
			US-78
			Tous
			Dupliquer une culture existante
			Réutiliser un itinéraire pour une nouvelle saison
			BASSE
### 🔍 Recherche et navigation
			ID
			En tant que...
			Je veux...
			Afin de...
			Priorité
			US-80
			Tous
			Rechercher parmi mes cultures
			Retrouver rapidement une culture spécifique
			MOYENNE
			US-81
			Tous
			Rechercher dans mes notes
			Retrouver des informations spécifiques
			BASSE
			US-82
			Tous
			Naviguer entre les différentes sections
			Utiliser toutes les fonctionnalités facilement
			HAUTE
			US-83
			Tous
			Avoir un bouton de retour contextuel
			Revenir à mon emplacement précédent
			HAUTE
			US-84
			Tous
			Accéder à l'aide en contexte
			Comprendre comment utiliser chaque fonctionnalité
			MOYENNE
### 📛 Avantages par type d'utilisateur
#### Pour les débutants
- Accompagnement détaillé à chaque étape
- Instructions simplifiées et vocabulaire accessible
- Conseils supplémentaires pour éviter les erreurs courantes
- Fiches techniques enrichies avec des explications détaillées
#### Pour les amateurs
- Interface plus concise et efficace
- Accès rapide aux informations techniques
- Flexibilité dans la personnalisation des itinéraires
- Focus sur l'organisation et l'optimisation des cultures