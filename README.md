# ☠️ Skull King – Journal de bord

Application web mobile (PWA) pour gérer les scores du jeu de plis **Skull King** : mises, plis gagnés, bonus, classement et tableau récapitulatif, le tout sur une seule page HTML sans dépendance ni serveur.

> Projet de fan, non officiel. *Skull King* est une marque de Grandpa Beck's Games. Cette application ne contient ni les règles complètes ni les illustrations du jeu.

## Fonctionnalités

- **2 modes de calcul** au choix au début de la partie :
  - **Skull King** (classique) : 20 pts par pli si la mise est exacte, pénalités sinon.
  - **Rascal** : 10 pts par carte distribuée, tout, moitié ou rien selon la précision.
- **Règle optionnelle Rascal « Boulet de canon »** : choix Chevrotine / Boulet de canon pour chaque joueur et chaque manche (15 pts par carte si la mise est exacte, sinon 0).
- **7 formats de partie** : Classique, Pas d'impair, Prêt au combat, Attaque éclair, Tir de barrage, Tourbillon, L'heure du dodo.
- **2 à 8 joueurs**, avec mémorisation des noms utilisés (et suppression possible).
- **Bonus** : 14 de couleur, 14 noir, sirènes, pirates et Skull King capturés, plus un ajustement libre par pas de 5 pour les règles maison.
- **Validation de la manche** avec contrôle du total des plis, et modification possible à tout moment d'une manche passée : les totaux sont recalculés immédiatement.
- **Classement en direct**, tableau récapitulatif et proclamation du « Capitaine des Sept Mers » en fin de partie.
- **Réglages** (⚙) : langue, taille de l'affichage (70 % à 150 %), nouvelle partie.
- **5 langues** : français (par défaut), anglais, espagnol, allemand, italien.
- **Hors ligne** une fois installée, et sauvegarde automatique de la partie en cours dans le `localStorage` du navigateur.

## Structure du dépôt

```
.
├── index.html            # Toute l'application (HTML + CSS + JavaScript)
├── manifest.webmanifest  # Manifeste PWA
├── sw.js                 # Service worker (mode hors ligne)
├── icons/
│   ├── icon-192.png
│   ├── icon-512.png
│   └── icon-maskable-512.png
└── README.md
```

## Utilisation

Ouvrez simplement `index.html` dans un navigateur, ou hébergez le dépôt (voir ci-dessous) et ouvrez l'adresse sur votre téléphone.

Pour l'installer comme une appli sur Android : Chrome → menu ⋮ → **Installer l'application**.

## Héberger avec GitHub Pages

1. Poussez les fichiers à la racine du dépôt.
2. Dans **Settings → Pages**, choisissez la branche `main` et le dossier `/ (root)`.
3. L'application est disponible sur `https://<utilisateur>.github.io/<depot>/`.

Le service worker et le manifeste exigent du **HTTPS**, ce que GitHub Pages fournit.

## Générer un APK Android avec PWABuilder

1. Hébergez l'application en HTTPS (GitHub Pages convient).
2. Rendez-vous sur [pwabuilder.com](https://www.pwabuilder.com) et saisissez l'adresse de l'application.
3. Lancez l'analyse, puis **Package for stores → Android**.
4. Choisissez l'APK pour une installation directe (l'AAB sert à la publication sur le Play Store) et conservez précieusement la clé de signature fournie.
5. Installez l'APK sur le téléphone en autorisant les sources inconnues.

## Mettre à jour l'application

Après une modification, changez le numéro de version du cache dans `sw.js` (`skull-king-v1` → `skull-king-v2`, etc.) pour que les appareils récupèrent la nouvelle version.

## Données

Tout est stocké localement dans le navigateur (`localStorage`) : noms enregistrés, langue, taille d'affichage et partie en cours. Aucune donnée n'est envoyée à un serveur. Les données ne sont pas partagées entre la version web et l'application installée, ni entre appareils.

## Technologies

HTML, CSS et JavaScript natifs, sans framework ni bibliothèque. Polices [Pirata One](https://fonts.google.com/specimen/Pirata+One), [Cinzel](https://fonts.google.com/specimen/Cinzel) et [Alegreya](https://fonts.google.com/specimen/Alegreya) via Google Fonts.

## Licence

À définir (par exemple MIT).
