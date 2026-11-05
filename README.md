# Comprendre et présenter le site TenZ

## 1. Le projet
Le dossier `fansite1` contient le site EGO de Romann. Ton mini-site TenZ est dans `fansite2`. L'accueil du groupe est `index.html`.

Tu as **6 pages HTML**, pas une seule : `fansite2.html` (accueil), `actualites.html`, `realisations.html`, `evenements.html`, `galerie.html`, `contact.html`.

## 2. Les deux CSS
- `styles.css` à la racine : couleurs principales, police, header, navigation, footer, cartes, grille et responsive. Ce sont les styles COMMUNS.
- `fansite2/fansite2.css` : photo de TenZ, grande introduction, bouton, formulaire et mise en forme du contenu spécifique.
- `fansite1/fansite1.css` : détails propres à EGO (photo de fond, texte, icônes). Le contenu et la structure du site de Romann sont conservés.

## 3. Lire le début de ton HTML, ligne par ligne
- `<!DOCTYPE html>` : indique au navigateur qu'on utilise HTML5.
- `<html lang="fr">` : la page est en français.
- `<head>` : informations sur la page que l'on ne voit pas comme contenu principal.
- `<meta charset="UTF-8">` : prend en charge les accents.
- `<meta name="viewport" ...>` : aide à adapter l'affichage au téléphone.
- `<title>` : texte de l'onglet dans le navigateur.
- `<link rel="stylesheet" href="../styles.css">` : charge le CSS commun ; `../` signifie remonter d'un dossier.
- `<link rel="stylesheet" href="fansite2.css">` : charge les styles propres à TenZ.
- `<body>` : ce qui est visible sur la page.

## 4. Les balises qui reviennent partout
- `<header>` : bandeau en haut du site.
- `<nav>` : menu de navigation.
- `<a href="actualites.html">Actualités</a>` : lien vers une autre page.
- `<main>` : contenu principal.
- `<section>` : partie de page avec un sujet.
- `<div>` : boîte de regroupement, sans rôle sémantique particulier.
- `<h1>` : titre principal ; `<h2>` : sous-titre ; `<p>` : paragraphe.
- `<img src="tenz.jpg" alt="Photo de TenZ">` : image et description alternative.
- `<footer>` : bandeau en bas ; il contient aussi les liens.
- `<article>` : bloc autonome de contenu, utilisé pour les cartes.

## 5. C'est quoi une classe ?
`<div class="carte">` applique à cette boîte les règles CSS de `.carte`.
Le point dans `.carte` veut dire que c'est un sélecteur de classe.

## 6. Comprendre le CSS
- `background-color: #111;` : fond presque noir.
- `color: white;` : texte blanc.
- `padding: 40px;` : espace intérieur.
- `margin: 20px;` : espace extérieur.
- `display: flex;` : place des éléments sur une même ligne (par défaut).
- `display: grid;` : organise des blocs en colonnes.
- `grid-template-columns: repeat(2, 1fr);` : deux colonnes de taille égale.
- `gap: 20px;` : espace entre les éléments.
- `border-radius: 12px;` : coins arrondis.
- `:hover` : style quand la souris survole un élément.
- `@media screen and (max-width: 900px)` : règles utilisées lorsque l'écran est étroit. Cela rend le site responsive.

## 7. Le formulaire de contact
- `<form>` regroupe les champs.
- `<label for="nom">` donne un intitulé au champ `id="nom"`.
- `<input type="email">` demande un e-mail.
- `<textarea>` sert à écrire plusieurs lignes.
- `required` rend un champ obligatoire.
- Le bouton n'envoie aucun vrai e-mail. Il manque un serveur pour cela.

## 8. Tester des changements par toi-même
1. Dans `fansite2.html`, change le titre `BIENVENUE DANS L’UNIVERS DE TENZ` puis enregistre avec Ctrl+S.
2. Actualise la page du navigateur avec F5.
3. Dans `styles.css`, change `background-color: #111;` en `background-color: #191919;` puis reviens à `#111`.
4. Dans `fansite2.css`, change la largeur de `.photo-tenz` et observe la différence.
5. Dans `actualites.html`, change une phrase et vérifie le résultat.

## 9. Phrase pour la présentation
« Nous avons un site d'accueil commun et un mini-site par personne. Mon mini-site est celui de TenZ dans le dossier fansite2. J'ai organisé mes informations en plusieurs pages accessibles dans le header et le footer. Les styles communs sont dans styles.css, et les détails propres à TenZ dans fansite2.css. Les pages sont liées avec des balises a et des chemins relatifs. »

## 10. Questions que le professeur pourrait poser
**Pourquoi deux fichiers CSS ?** Pour éviter de répéter le design commun et garder les styles particuliers de chaque sujet.
**Pourquoi `../styles.css` ?** Car le HTML est dans le sous-dossier `fansite2` : `../` remonte au dossier parent.
**À quoi sert `class` ?** À cibler un élément HTML depuis le CSS.
**Quelle différence entre `margin` et `padding` ?** Margin = extérieur, padding = intérieur.
**Pourquoi header et footer ?** Pour naviguer en haut et en bas de chaque page, comme demandé.
**C'est quoi responsive ?** Adapter l'affichage au téléphone grâce à `@media`.
**Est-ce que le formulaire envoie vraiment ?** Non, c'est une maquette HTML.

## 11. À vérifier avant de rendre
- Remplir le mini-site `fansite3` : pour l'instant, le travail d'Ilyan est vide dans le ZIP reçu.
- Les liens du site EGO vers ses pages secondaires pointent vers des fichiers non fournis dans le ZIP reçu : Romann doit les ajouter.
- Vérifier les trois mini-sites sur téléphone et tester tous les liens.
- Préparer vos slides pour la présentation.
