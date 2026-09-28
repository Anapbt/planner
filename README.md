# Planner

Planner de la semaine : tâches par jour et par catégorie, tâches de la semaine, repas du midi et du soir.
Web app installable sur iPhone, qui fonctionne hors ligne. Les données restent sur le téléphone (stockage local du navigateur).

## Mettre en ligne sur GitHub Pages

1. Crée un repo public, par exemple `planner`, et pousse le contenu de ce dossier à la racine :
   ```bash
   git init && git add . && git commit -m "Planner"
   git branch -M main
   git remote add origin git@github.com:TON-PSEUDO/planner.git
   git push -u origin main
   ```
2. Sur GitHub : **Settings → Pages → Build and deployment**, source **Deploy from a branch**, branche `main`, dossier `/ (root)`.
3. Après une minute, l'app est disponible sur `https://TON-PSEUDO.github.io/planner/`.

## Installer sur l'iPhone

1. Ouvre l'adresse dans **Safari**.
2. Touche **Partager** puis **Sur l'écran d'accueil**, et valide.
3. Lance l'app depuis son icône : elle s'ouvre en plein écran et fonctionne hors ligne.

Utilise toujours l'icône de l'écran d'accueil : les données de l'app installée sont séparées de celles de Safari.

## Utilisation

- Toucher une tâche la coche ou la décoche.
- Appui long sur une tâche pour la supprimer.
- Toucher la plage de dates en haut de la vue semaine ramène à la semaine en cours.
- « Nouvelle catégorie » dans l'écran d'ajout crée une catégorie, réutilisable ensuite.

## Mettre à jour l'app

Après une modification, change la valeur de `CACHE` dans `sw.js` (par exemple `planner-v2`) avant de pousser.
La nouvelle version apparaît au lancement suivant (parfois il faut fermer et rouvrir l'app deux fois).
Tes données ne sont pas touchées par les mises à jour.
