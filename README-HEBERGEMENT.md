# Héberger le menu MBOLO GRILL sur Render

Ce dossier contient le site prêt à publier : `index.html`, ses 15 photos dans `images/` et `render.yaml` pour Render Blueprint.

## Déploiement recommandé avec GitHub

1. Décompressez cette archive sur votre ordinateur.
2. Créez un dépôt GitHub et ajoutez **le contenu** du dossier `render-mbolo` à la racine du dépôt. Le fichier `render.yaml` et `index.html` doivent être à la racine.
3. Dans Render, choisissez **New + → Blueprint** et connectez ce dépôt GitHub.
4. Render détectera `render.yaml`. Validez la création du service statique `mbolo-grill-menu`.
5. Une fois le déploiement terminé, ouvrez l’URL `onrender.com` affichée par Render.

## Déploiement sans Blueprint

Créez un **Static Site** dans Render, connectez le dépôt, puis indiquez :

- **Build Command** : `echo "Site statique prêt"`
- **Publish Directory** : `.`

Le site ne nécessite ni base de données, ni dépendances, ni commande de démarrage Node/Python. L’interactivité (navigation, fiches plats et panier) est incluse dans la page.
