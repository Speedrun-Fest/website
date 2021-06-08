# speedrunfest-website
Site Internet pour l'événement Game* Speedrun Fest.

## Prérequis
* Le site est entièrement en HTML/CSS, avec un soupçon de JS, donc pas de prérequis particulier.
* Ne pas oublier de payer le nom de domaine si pas déjà fait.

## Guidelines
* Le site Internet se met automatiquement à jour à chaque push sur la branche master.
* Pour chaque édition, créer une nouvelle branche à partir du Master.
    * Les branches doivent être nommées selon l'année de l'édition.
    * Les branches des années passées servent d'archive.
    * Modifier directement la branche concernée, puis push dans la branche master. Éviter d'aller dans l'autre sens dans la mesure du possible.
* Pour chaque édition, tenter de trouver un thème et une palette de couleur sympathique.
    * Ne pas hésiter à adapter la petite mascotte au mood des gens.
* Dans la mesure du possible, essayer de simplifier la maintenance d'année en année (voir "[Fichier `album.css`](#fichier-albumcss)".

## Utilisation
### Éléments fournis dans le dossier `img/`
* Pour chaque réseau social (Discord, Facebook, Instagram, Telegram, Twitch, Twitter), il existe une version noire et une version blanche (`_w`). Il suffit de changer dans `index.html` directement.
* Les logos (`game-logo.png` et `header.png`) sont à recoloriser suivant la palette de couleur.
* Le fond (`bg.png`) peut être modifié directement.

### Fichier `index.html`
Il s'agit du coeur de la page. Normalement, les modifications sont assez simples, mais en cas de besoin, se référer à des [petits tutoriels en ligne](https://www.freecodecamp.org/news/want-to-learn-to-build-websites-try-our-free-4-hour-crash-course-on-html-css-2/).

Choses à modifier d'année en année et à ne pas oublier :
* Dans `meta name="description"`, préciser les dates et les activités.
* Dans `title`, changer les dates.
* Faire une jolie `<!-- Introduction -->`.
* Dans `<!-- Petites icones -->`, changer les informations en fonction des besoins.
* Mettre à jour les `<!-- Horaires -->`.
    * En gros, tout le contenu dans chaque paire `<li>`/`</li>` correspond à une plage horaire.
    * Note : dans la branche `2020`, il existe une versions à trois colones pour trois jours, et dans la branche `2021` une version à une colonne pour un jour. Ne pas hésiter à s'en inspirer.
* Changer la date dans le `<!-- Footer -->`.

### Fichier `album.css`
La plupart des images/couleurs peuvent être modifiées directement depuis le fichier `album.css`, tout en haut. Toutes les variables à modifier sont tout en haut du fichier, sous `:root`. Le site est fait pour être vitrine et indicatif, mais ne pas hésiter à ajouter des éléments si nécessaire.

Subtilités :
* Il est possible de choisir un fond uni ou bien une image de fond. Dans ce cas, dans l'élément `body`, il faut [commenter la ligne correspondante](https://developer.mozilla.org/fr/docs/Web/CSS/Comments), et décommenter l'autre.
* Il existe plusieurs petites icônes tout en haut du site avec du texte. Il est possible de leur attribuer une image pour chaque, en modifiant (de gauche à droite) `--icon-target`, `--icon-time`, et `--icon-online`

## Besoin d'aide ?
Contacter les ancien·ne·s contributeur·trice·s, et ça devrait bien se passer.
