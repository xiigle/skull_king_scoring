# ☠️ Scorekeeper for Skull King

Application mobile pour gérer les scores du jeu de plis **Skull King** : mises, plis gagnés, bonus, classement et tableau récapitulatif.

> Projet de fan, non officiel et sans lien avec Grandpa Beck's Games. *Skull King* est une marque de son propriétaire.

## Fonctionnalités

- **Deux modes de calcul** : Skull King (classique) et Rascal, avec la règle optionnelle « Boulet de canon ».
- **Sept formats de partie** : classique (10 manches), Pas d'impair, Prêt au combat, Attaque éclair, Tir de barrage, Tourbillon, L'heure du dodo.
- **2 à 8 joueurs**, avec mémorisation des noms.
- **Manche en deux temps** : validation des mises (avec le total par rapport au nombre de plis), puis validation de la manche.
- **Corrections possibles à tout moment**, signalées par ✎ quand elles ont lieu après validation.
- **Bonus** : 14, sirènes, pirates, Skull King et ajustement libre par pas de 5.
- **5 langues** : français, anglais, espagnol, allemand, italien.
- **Taille d'affichage réglable** (70 % à 150 %).
- **Fonctionne hors ligne** et sauvegarde automatiquement la partie en cours.

## Utilisation

### Sur Android (APK)

1. Ouvrez la page [Releases](../../releases) du dépôt et téléchargez le fichier `.apk` de la dernière version.
2. Ouvrez-le sur le téléphone et autorisez l'installation depuis cette source si Android le demande.
3. Lancez l'appli.

### Dans un navigateur

Ouvrez simplement le fichier `index.html` dans un navigateur (téléphone ou ordinateur). Aucune installation ni connexion n'est nécessaire, hormis le chargement des polices (voir ci-dessous).

## Données

Les noms enregistrés, la langue, la taille d'affichage et la partie en cours sont stockés localement sur l'appareil. Rien n'est envoyé sur Internet. Ces données sont propres à chaque appareil et à chaque navigateur, et elles sont effacées si l'appli est désinstallée.

## Polices

La version HTML charge les polices *Pirata One*, *Cinzel* et *Alegreya* depuis Google Fonts. Hors connexion, elle utilise une police de secours. L'APK embarque ses polices.
