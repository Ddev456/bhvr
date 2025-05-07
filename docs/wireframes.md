# Wireframes textuels – Carnet Potager 🌱

> Ces wireframes textuels décrivent la structure des écrans clés du MVP, pour guider le développement et la conception UI/UX. À adapter lors de la réalisation de maquettes graphiques (Penpot, Figma, etc.).

---

## 1. Onboarding utilisateur

**Écran 1 : Bienvenue**
- Logo + nom de l'app
- Slogan court
- Bouton "Créer un compte" / "Se connecter"

**Écran 2 : Création de compte**
- Champ email
- Champ mot de passe
- Bouton "Valider"
- Lien "Déjà un compte ?"

**Écran 3 : Configuration profil**
- Sélecteur niveau (Débutant/Amateur)
- Sélecteur région (dropdown ou auto via géoloc)
- Jours préférés de jardinage (checkbox)
- Bouton "Continuer"

**Écran 4 : Confirmation**
- Message de bienvenue personnalisé
- Bouton "Commencer" (redirige vers dashboard)

---

## 2. Assistant interactif (création d'itinéraire)

**Écran 1 : Lancer l'assistant**
- Bouton "Nouvelle culture" sur le dashboard

**Écran 2 : Sélection de la plante**
- Barre de recherche
- Liste de suggestions (cartes ou liste)
- Sélection plante → bouton "Suivant"

**Écran 3 : Choix de la zone de culture**
- Liste des zones existantes (cartes)
- Bouton "Ajouter une zone" si besoin
- Sélection zone → bouton "Suivant"

**Écran 4 : Point de départ**
- Radio : "Semis", "Plants achetés", "Autre"
- Champ optionnel : variété
- Bouton "Générer mon itinéraire"

**Écran 5 : Résumé & validation**
- Timeline générée (aperçu)
- Bouton "Valider"

---

## 3. Dashboard synthétique

- Header : "Mon potager" + accès profil
- Bouton "Nouvelle culture" (lance assistant)
- Liste des cultures actives (cartes)
  - Nom plante, zone, statut, prochaine tâche
  - Bouton "Voir détails"
- Section "Tâches du jour" (liste)
- Statistiques rapides (nb cultures, tâches à faire)

---

## 4. Fiche culture (vue détaillée)

- Header : Nom plante + zone
- Onglets :
  - "Fiche technique" (infos, conseils, besoins)
  - "Carnet de bord" (notes, photos, réussites/échecs)
  - "Itinéraire" (timeline interactive)
- Bouton retour dashboard

---

## 5. Timeline interactive

- Header : "Itinéraire de culture"
- Frise horizontale (semaines/mois)
- Cartes tâches (à faire, en cours, fait)
  - Nom tâche, date, statut, bouton "Valider"
- Bouton "Ajouter une tâche"
- Bouton retour fiche culture

---

## 6. Ajouts futurs (hors MVP)

- Plan du jardin interactif (drag&drop, cartographie)
- Notifications push
- Partage communautaire

---

> Pour les schémas visuels, voir `/docs/assets/` (à compléter avec Penpot ou autre outil graphique). 