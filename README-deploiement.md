# CTM Blog V4 — Auto-scan (Ultra Pro)

Base URL
https://clprepas.com/blog/

## Objectif
- index.html premium CTM
- Recherche + filtres + tri + pagination
- articles.json généré automatiquement par script (local)

## Déploiement cPanel
1) Uploader le ZIP dans /public_html/blog/
2) Extraire
3) Ouvrir https://clprepas.com/blog/

## Auto-scan (local)
1) Mettre vos dossiers d’articles dans un dossier /blog local
2) Lancer:
   python scripts/generate-articles.py --blog-dir "C:\xampp\htdocs\blog" --base-url "https://clprepas.com/blog"
3) Uploader le nouveau articles.json sur le serveur

## Notes images
- Le blog utilise l'image définie dans articles.json.
- Si l'image n'existe pas, fallback automatique: /blog/assets/img/hero.jpg
- OG global: /blog/assets/img/og.jpg
