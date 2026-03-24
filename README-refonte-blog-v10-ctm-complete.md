# Refonte blog CTM signature — pack final

Ce pack contient la reconstruction complète du blog à partir des vrais dossiers d’articles.

## Ce qui a été fait

- intégration des articles qui n’apparaissaient pas dans le blog par création des `meta.json` manquants
- reconstruction de `api/posts.php` avec un mode de secours qui sait lire les pages HTML si un `meta.json` manque encore plus tard
- couverture uniforme du blog avec `assets/img/cover-default-signature.svg`
- image Open Graph par défaut commune à tout le blog : `assets/img/og-cover-default-signature.png`
- harmonisation des pages d’articles par ajout d’une signature CTM premium commune
- mise à jour uniforme des balises `canonical`, `og:*` et `twitter:*`
- régénération de `data/posts-fallback.json`

## Fichiers clés

- `assets/article-signature.css`
- `assets/article-signature.js`
- `assets/img/og-cover-default-signature.png`
- `api/posts.php`
- `data/posts-fallback.json`

## Déploiement

Déposez le contenu de ce ZIP dans `/public_html/blog/` en remplaçant les fichiers existants.

## Vérifications utiles

- ouvrir `/blog/`
- vérifier l’apparition des nouveaux articles dans l’accueil
- vérifier `/blog/categories/`
- vérifier `/blog/archives/`
- ouvrir 4 à 5 articles et contrôler la nouvelle bannière signature CTM
- tester le partage Facebook avec la même image OG par défaut
