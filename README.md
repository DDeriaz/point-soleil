# Point Soleil

Calcul du point astronomique au Soleil à partir de la lecture brute du sextant.

**Utiliser l'application :** https://votre-nom.github.io/point-soleil/
Sur iPhone : Safari → Partager → « Sur l'écran d'accueil ».
Sur Android : Chrome → menu ⋮ → « Installer l'application ».
Une fois installée, elle fonctionne sans connexion.

## Ce qu'elle fait
- Lecture brute du sextant (angle double) : soustraction du zéro et division par deux
- Horizon de mer ou horizon artificiel ; bord inférieur, supérieur ou centre du Soleil
- Corrections de dépression, réfraction, demi-diamètre et parallaxe
- Éphémérides du Soleil calculées, sans almanach (précision ≈ 0,6′)
- Méthode de l'intercept (Marcq Saint-Hilaire) ; point par moindres carrés avec plusieurs visées
- Contrôle de cohérence par l'intercept de chaque visée

## Limites
- L'observateur est supposé immobile entre les visées (pas de transport de droite).
- Une seule visée donne une droite de position, pas un point.

Calculs portés d'un script R (`point_astro.R`).
