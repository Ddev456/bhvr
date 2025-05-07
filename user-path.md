# Parcours utilisateurs – Carnet Potager 🌱

> Ce document détaille les principaux parcours utilisateurs du MVP, avec wireframes textuels, liens vers les user stories, alternatives et moments critiques. Il sert de référence UX pour le développement.

---

## 📋 Qu'est-ce qu'un parcours utilisateur ?
Un parcours utilisateur est une séquence d'étapes permettant d'atteindre un objectif clé. Chaque étape est liée à des user stories ([voir user-stories.md](user-stories.md)).

---

## 🌱 Parcours 1 : Première connexion et configuration initiale
**Persona** : Julie, 32 ans, citadine débutante avec un petit balcon

### Étapes & wireframes textuels
1. **Inscription et création de compte**  
   _US-01, US-02_  
   Wireframe : [Onboarding – Écran 2](docs/wireframes.md)
2. **Onboarding initial**  
   _US-03, US-04, US-05, US-06_  
   Wireframe : [Onboarding – Écran 3]
3. **Création de la première zone de culture**  
   _US-10, US-11, US-12, US-13, US-14, US-17_  
   Wireframe : [Gestion des zones]
4. **Tutoriel guidé des fonctionnalités principales**  
   _US-20, US-30, US-50_  
   Wireframe : [Dashboard, Assistant, Fiche culture]

**Moments critiques** :
- Si la liste des types de sol est trop technique pour une débutante
- Si le processus d'onboarding est trop long

**Alternatives** :
- Proposer un mode "découverte rapide"

---

## 🌿 Parcours 2 : Création d'un itinéraire de culture avec l'assistant
**Persona** : Julie, souhaite cultiver des tomates cerises sur son balcon

### Étapes & wireframes textuels
1. **Accès à l'assistant**  
   _US-20_  
   Wireframe : [Dashboard, bouton "Nouvelle culture"]
2. **Sélection de la plante**  
   _US-22_  
   Wireframe : [Assistant – Écran 2]
3. **Choix de la zone de culture**  
   _US-21_  
   Wireframe : [Assistant – Écran 3]
4. **Point de départ**  
   _US-23, US-24_  
   Wireframe : [Assistant – Écran 4]
5. **Génération et visualisation de l'itinéraire**  
   _US-27_  
   Wireframe : [Assistant – Écran 5, Timeline]
6. **Consultation de la fiche technique**  
   _US-30, US-31, US-32, US-33, US-34_  
   Wireframe : [Fiche culture]
7. **Confirmation et première tâche**  
   _US-51_  
   Wireframe : [Timeline]

**Moments critiques** :
- Si l'itinéraire généré est trop technique
- Si la timeline n'est pas intuitive

**Alternatives** :
- Proposer un mode "débutant" avec explications détaillées

---

## 🔍 Parcours 3 : Suivi quotidien des cultures
**Persona** : Marc, 60 ans, retraité avec expérience

### Étapes & wireframes textuels
1. **Consultation du dashboard**  
   _US-70, US-73_  
   Wireframe : [Dashboard]
2. **Filtrage par zone**  
   _US-71_  
   Wireframe : [Dashboard, filtre]
3. **Accès à une tâche spécifique**  
   _US-65_  
   Wireframe : [Timeline, carte tâche]
4. **Réalisation et validation de la tâche**  
   _US-51_  
   Wireframe : [Timeline, bouton "Valider"]
5. **Ajout d'une note et photo**  
   _US-40, US-41_  
   Wireframe : [Carnet de bord]
6. **Adaptation du planning**  
   _US-53, US-64_  
   Wireframe : [Timeline, drag&drop]
7. **Consultation des statistiques**  
   _US-75_  
   Wireframe : [Dashboard, stats]

**Moments critiques** :
- Si la validation de tâche est trop complexe
- Si l'ajout de note/photo est peu intuitif

**Alternatives** :
- Accès rapide à l'ajout de note/photo depuis la timeline

---

## 🔄 Parcours 4 : Modification d'un itinéraire existant
**Persona** : Marc souhaite ajuster l'itinéraire de ses tomates

### Étapes & wireframes textuels
1. **Accès à l'itinéraire existant**  
   _US-74, US-50_  
   Wireframe : [Dashboard, Fiche culture, Timeline]
2. **Navigation vers l'onglet itinéraire**  
   _US-50_  
   Wireframe : [Fiche culture, onglet "Itinéraire"]
3. **Ajout d'une nouvelle tâche**  
   _US-54_  
   Wireframe : [Timeline, bouton "Ajouter une tâche"]
4. **Suppression d'une tâche**  
   _US-55_  
   Wireframe : [Timeline, carte tâche]
5. **Modification d'une date de tâche**  
   _US-53, US-64_  
   Wireframe : [Timeline, drag&drop]
6. **Consultation des impacts**  
   _US-56_  
   Wireframe : [Timeline, détails tâche]
7. **Validation des changements**  
   _US-50_  
   Wireframe : [Timeline, bouton "Valider"]

**Moments critiques** :
- Si les modifications créent des conflits
- Si le drag&drop n'est pas précis sur mobile

**Alternatives** :
- Proposer un mode "annuler/valider" avant sauvegarde

---

## 📒 Parcours 5 : Consultation et enrichissement d'une fiche technique
**Persona** : Julie, débutante, recherche des infos sur la culture des tomates cerises

### Étapes & wireframes textuels
1. **Accès à la fiche technique**  
   _US-30_  
   Wireframe : [Dashboard, Fiche culture]
2. **Navigation dans les sections d'information**  
   _US-31, US-32, US-33, US-34_  
   Wireframe : [Fiche culture, onglet "Fiche technique"]
3. **Ajout d'une note personnelle**  
   _US-40_  
   Wireframe : [Carnet de bord]
4. **Consultation des associations**  
   _US-32_  
   Wireframe : [Fiche culture, section associations]

**Moments critiques** :
- Si les infos techniques sont trop complexes
- Si la fiche technique manque de hiérarchisation

**Alternatives** :
- Proposer des "conseils débutant" en haut de chaque section

---

## Liens utiles
- [user-stories.md](user-stories.md) : User stories détaillées et priorisées
- [features.md](features.md) : Fonctionnalités détaillées
- [docs/wireframes.md](docs/wireframes.md) : Wireframes textuels