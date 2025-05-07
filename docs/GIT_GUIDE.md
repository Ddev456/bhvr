# Guide Git & GitHub pour le projet `bhvr` 🦫

> **Notes pour adopter une méthodologie professionnelle avec Git et GitHub sur ce monorepo TypeScript.**

---

## 🚦 Workflow Git Professionnel

1. **Fork & Clone** :
   - Forker le repo sur GitHub si besoin, puis le cloner :
     ```bash
     git clone https://github.com/<votre-utilisateur>/bhvr.git
     cd bhvr
     ```
2. **Branche dédiée** :
   - Créer une branche pour chaque fonctionnalité/correctif :
     ```bash
     git checkout -b feat/ma-fonctionnalite
     ```
3. **Commits atomiques** :
   - Faire des commits petits, clairs et fréquents.
4. **Push & Pull Request** :
   - Pousser la branche et ouvrir une Pull Request (PR) sur GitHub.
5. **Code Review** :
   - "Demander une review", commentaires, puis "merger"/fusionner après validation.
6. **Mise à jour régulière** :
   - Garder la branche à jour avec `main` :
     ```bash
     git fetch origin
     git rebase origin/main
     # ou
     git merge origin/main
     ```

---

## 🔥 Commandes Git Essentielles

| Action                        | Commande                                    |
|------------------------------|---------------------------------------------|
| Cloner le repo               | `git clone <url>`                           |
| Créer une branche            | `git checkout -b feat/ma-fonctionnalite`    |
| Lister les branches          | `git branch -a`                             |
| Voir le statut               | `git status`                                |
| Ajouter des fichiers         | `git add <fichier>`                         |
| Committer                    | `git commit -m "feat: ajout de X"`         |
| Modifier le dernier commit   | `git commit --amend`                        |
| Pousser une branche          | `git push origin <ma-branche>`              |
| Récupérer les changements    | `git pull`                                  |
| Fusionner une branche        | `git merge <autre-branche>`                 |
| Rebaser sur main             | `git rebase main`                           |
| Afficher l'historique        | `git log --oneline --graph --all`           |

---

## 📝 Types de messages de commit (Conventional Commits)

Adopter le format [Conventional Commits](https://www.conventionalcommits.org/) :

```
<type>[optional scope]: <description>

[optional body]
[optional footer]
```

### Types courants :
- `feat` : Nouvelle fonctionnalité
- `fix` : Correction de bug
- `docs` : Documentation
- `style` : Formatage, indentation, etc. (pas de code modifié)
- `refactor` : Refactoring sans ajout de fonctionnalité
- `test` : Ajout/modif de tests
- `chore` : Tâches diverses (build, outils, etc.)

### Exemples :
- `feat(client): ajout du bouton de connexion`
- `fix(server): corrige le crash lors du login`
- `docs: améliore le README`
- `refactor(shared): simplifie la gestion des types`

---

## 🌳 Stratégie de branches

- `main` : branche de production, toujours stable
- `dev` *(optionnel)* : intégration continue, avant merge sur `main`
- `feat/xxx` : nouvelle fonctionnalité
- `fix/xxx` : correctif
- `docs/xxx` : documentation

> **Note** : Préfixer les branches pour plus de clarté !

---

## ✅ Bonnes pratiques

- **Un commit = une idée** : éviter les commits fourre-tout.
- **Messages clairs** : explicites, en anglais ou français cohérent.
- **Relire les PRs** avant la review ?
- **Pas de code mort** ou de secrets dans le repo !
- **Utiliser `.gitignore`** pour éviter de versionner les fichiers sensibles ou inutiles.

---

## 🛠️ Outils

- ?? [GitHub Desktop](https://desktop.github.com/) : interface graphique simple ??
- ?? [GitKraken](https://www.gitkraken.com/) : gestion avancée des branches ??
- ?? [VSCode GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) : historique ... dans VSCode

---

## 📚 Ressources utiles

- [Pro Git Book (FR)](https://git-scm.com/book/fr/v2)
- [GitHub Docs](https://docs.github.com/fr)
- [Conventional Commits](https://www.conventionalcommits.org/fr/v1.0.0/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

---

> _Happy coding & commit responsibly!_ 