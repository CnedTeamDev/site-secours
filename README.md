# Site de Secours — Cned

Bienvenue sur le dépôt de la page de secours du Cned.  
Ce site statique permet d’informer parents, élèves et équipes en cas d’incident majeur sur les plateformes habituelles.

## 📁 Structure principale

- `_posts/` : tous les messages d’alerte, d’info ou de consignes (format `YYYY-MM-DD-titre.md`)
- `_layouts/`, `assets/`, `index.html` : gabarits, images et page d’accueil.

## ✍️ Ajouter une actualité (post)

1. Créer un fichier dans `_posts/` au format :

   ```
   YYYY-MM-DD-titre.md
   ```

   Exemple :

   ```
   _posts/2026-04-17-info-examens.md
   ```

2. Respecter la structure suivante :

   ```markdown
   ---
   title: "Titre affiché"
   date: YYYY-MM-DD HH:MM:SS +0200
   type: erreur | info | warning | neutre
   ---

   Message rédigé en langage clair, sans jargon technique.
   ```

3. Les nouveautés s’affichent automatiquement sur la page d’accueil.

## ⚠️ Important : gestion des dates

- **N’utilisez jamais de date future** dans le nom ou l’en-tête d’un post si l’annonce concerne un incident immédiat.
- Les fichiers datés dans le futur ne seront pas affichés tant que la date n’est pas atteinte.
- Pour des annonces planifiées, pensez à bien vérifier la date/heure avant de publier.

## ℹ️ Types de posts

Utilisez la propriété `type` selon le contexte :

- `erreur` — Anomalie, panne constatée
- `info` — Retour à la normale, consigne générale
- `warning` — Sécurité, vigilance, examens
- `neutre` — Messages rassurants, fausse alerte

## 🚀 Publication

Toute modification dans `_posts/` apparaît sur le site après validation de la branche principale (main).  
Les pages se mettent à jour automatiquement.

## 👥 Pour aller plus loin

- [Documentation Jekyll (FR)](https://jekyllrb.com/docs/)
