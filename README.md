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
