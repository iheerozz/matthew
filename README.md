# Outils de classe — St. Matthew

Petite collection d'outils que j'utilise en cours de français et en A Level
Business 9609. Tout est en HTML, CSS et JavaScript, sans dépendance ni serveur :
chaque fichier s'ouvre tel quel dans un navigateur.

## Contenu

| Fichier | Rôle |
|---|---|
| `index.html` | Page d'accueil, barre d'onglets, sauvegarde automatique |
| `jigsaw.html` | Onglet Jigsaw (deux sous-onglets) |
| `jigsaw-business.html` | Méthode Jigsaw — A Level Business 9609 (11A/11B/11C) |
| `jigsaw-francais.html` | Méthode Jigsaw — français (9A à 10C) |
| `participation.html` | Suivi de participation, tirage au sort, historique par séance |
| `calendar.html` | Mon emploi du temps de la semaine |
| `annee.html` | Calendrier scolaire 2026–2027 |
| `exercices.html` | Onglet Exercices (deux sous-onglets) |
| `ex-avoir-etre.html` | Expressions avec avoir et être — exercice interactif |
| `quiz-avoir-etre.html` | Le même quiz, version à imprimer (4 billets par page) |
| `jeux.html` | Onglet Jeux (deux sous-onglets) |
| `plateau.html` | Le Plateau des 25 défis |
| `miniz-presentation-3.html` | MiniZ Présentation |

## Comment c'est construit

`index.html` affiche la barre d'onglets et charge chaque outil dans un cadre.
Trois onglets ont leurs propres sous-onglets : Jigsaw, Exercices et Jeux.
Un outil n'est chargé qu'au premier clic, et il reste en mémoire ensuite, donc
on peut passer d'un onglet à l'autre sans perdre une séance en cours.

Les données (points de participation, présences, thèmes du jour, horaires
modifiés) sont enregistrées dans le navigateur. Une copie de sécurité part
automatiquement dans une seconde base du navigateur, et le bouton en haut à
droite permet en plus d'écrire dans un fichier sur le disque.

## Mettre en ligne avec GitHub Pages

1. Déposer tous les fichiers à la racine du dépôt.
2. Settings → Pages.
3. Source : « Deploy from a branch », branche `main`, dossier `/ (root)`.
4. Attendre une minute, puis ouvrir l'adresse affichée.

Les liens entre fichiers sont tous relatifs, donc le site fonctionne aussi bien
à la racine que dans un sous-dossier.

## Un point à savoir sur les données

Le navigateur range les données par adresse de site. Un même outil ouvert sur
deux adresses différentes a donc deux jeux de données séparés, et il en va de
même entre l'ordinateur et le téléphone.

Avant de cliquer sur « Sauvegarde » depuis une nouvelle adresse, mieux vaut
faire une copie du fichier JSON existant : le sélecteur de fichier écrase le
fichier choisi.
