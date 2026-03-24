# Refonte blog CTM signature — V11 éditoriale

Ce pack prolonge la base V10 en ajoutant une passe éditoriale sur l’intérieur des articles tout en conservant la signature visuelle CTM, la cover uniforme et l’image Open Graph commune.

## Ce qui a été fait

- harmonisation éditoriale de l’intérieur des pages article
- ajout de repères de lecture, plan d’article, synthèse finale et CTA homogènes
- traitement renforcé de 10 articles piliers
- correction des URL internes non sécurisées de `http` vers `https` quand elles pointaient vers `clprepas.com`
- mise à jour des `meta.json` avec auteur, URL canonique et extraits nettoyés
- régénération de `data/posts-fallback.json`
- légère montée en gamme de l’accueil, des catégories et des archives via `blog-v11.css` et `blog-v11.js`

## Fichiers clés

- `assets/article-signature.css`
- `assets/article-signature.js`
- `assets/blog-v11.css`
- `assets/blog-v11.js`
- `api/posts.php`
- `data/posts-fallback.json`
- `journal-modifications-v11.md`

## Déploiement

Déposez le contenu du ZIP dans `/public_html/blog/` en remplaçant les fichiers existants.

## Vérifications utiles

- ouvrir `/blog/`
- ouvrir `/blog/categories/`
- ouvrir `/blog/archives/`
- tester 4 à 5 articles standards
- tester les 10 articles piliers
- vérifier qu’aucun lien interne `http://clprepas.com` ne subsiste dans les pages déployées
- tester l’aperçu social de 2 articles pour confirmer l’OG par défaut uniforme
