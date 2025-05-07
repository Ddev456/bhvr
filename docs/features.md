# Fonctionnalités du MVP – Carnet Potager 🌱

> Ce document liste les fonctionnalités principales du MVP, avec priorités, critères d'acceptation, tags MVP, et liens vers les user stories. Il sert de référence directe pour le développement.

---

## 📋 Vue d'ensemble des fonctionnalités

| Fonctionnalité                | Description                                      | Limite MVP         | Priorité   | User Stories |
|-------------------------------|--------------------------------------------------|--------------------|------------|--------------|
| 🤖 Assistant interactif       | Génère des itinéraires de culture personnalisés   | Oui                | Essentiel  | US-20 à US-28 |
| 🗂️ Gestion des zones          | Création et gestion de zones de culture           | Max 5 zones        | Essentiel  | US-10 à US-17 |
| 📒 Carnet de culture          | Fiches techniques, carnet de bord, timeline       | Oui                | Essentiel  | US-30 à US-56 |
| ⏳ Timeline interactive        | Visualisation et gestion des tâches               | Oui                | Essentiel  | US-50 à US-66 |
| 📊 Dashboard                  | Vue synthétique de toutes les cultures et zones   | Oui                | Important  | US-70 à US-76 |
| 🔍 Recherche                  | Recherche parmi cultures, notes                   | Non (hors MVP)     | Optionnel  | US-80 à US-81 |
| 🛎️ Notifications              | Alertes pour tâches à venir                      | Non (hors MVP)     | Optionnel  | -            |
| 🗺️ Plan du jardin             | Visualisation cartographique, drag&drop           | Non (hors MVP)     | Optionnel  | -            |
| 👥 Partage communautaire       | Partage de cultures, entraide                     | Non (hors MVP)     | Optionnel  | -            |

---

## Critères d'acceptation par fonctionnalité clé

### 🤖 Assistant interactif *(Essentiel, MVP)*
- L'utilisateur peut lancer l'assistant depuis le dashboard
- L'assistant pose les questions nécessaires (plante, zone, point de départ, variété)
- Un itinéraire personnalisé est généré et affiché
- L'utilisateur peut valider ou modifier l'itinéraire
- **User Stories** : US-20 à US-28

### 🗂️ Gestion des zones *(Essentiel, MVP)*
- L'utilisateur peut créer, éditer, supprimer jusqu'à 5 zones
- Chaque zone a un nom, un type, une exposition, des dimensions, un type de sol
- Les zones sont sélectionnables dans l'assistant
- **User Stories** : US-10 à US-17

### 📒 Carnet de culture *(Essentiel, MVP)*
- Chaque culture a une fiche technique générée automatiquement
- L'utilisateur peut ajouter des notes, photos, réussites/échecs
- L'historique est consultable par culture
- **User Stories** : US-30 à US-45

### ⏳ Timeline interactive *(Essentiel, MVP)*
- L'utilisateur visualise les tâches sur une frise temporelle
- Il peut valider, modifier, ajouter ou ignorer des tâches
- Drag & drop pour réorganiser les tâches (si temps)
- **User Stories** : US-50 à US-66

### 📊 Dashboard *(Important, MVP)*
- Vue d'ensemble des cultures, zones, tâches à venir
- Accès rapide à l'assistant et aux fiches cultures
- Statistiques de progression
- **User Stories** : US-70 à US-76

---

## Limites/scope du MVP
- Maximum 10 itinéraires de culture par utilisateur
- Maximum 5 zones de culture
- Pas de notifications push
- Pas de plan du jardin interactif
- Pas de partage entre utilisateurs

---

## Liens utiles
- [user-stories.md](user-stories.md) : User stories détaillées et priorisées
- [README.md](README.md) : Synthèse MVP, roadmap, checklist
- [docs/wireframes.md](docs/wireframes.md) : Wireframes textuels