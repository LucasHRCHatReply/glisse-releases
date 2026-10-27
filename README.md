# Glisse pour macOS

Glisse ajoute une couche de gestes à la barre de titre des fenêtres : deux ou trois doigts qui glissent ou pincent sur
une barre de titre calent la fenêtre (moitié, tiers, agrandie, centrée), la passent en plein écran, la minimisent ou la
ferment. L'app vit dans la barre des menus (petite main). Aucun compte, aucune licence, aucune télémétrie.

- **Aperçu** : pendant le geste, une affiche près du curseur montre l'écran en miniature avec la zone choisie, et la zone s'éclaire ;
  la fenêtre y va au relâchement, et revenir au point de départ annule.
- **Zones** : moitiés, quarts (glissements en diagonale), tiers, deux tiers, huitièmes, agrandir, centrer, plein écran.
- **Fenêtre** : écarter ou pincer, glisser à 3 doigts : plein écran, minimiser, fermer.
- **Dock** : les mêmes gestes sur l'icône d'une app, dans le Dock.
- **Groupes** : ⌃⌥G groupe plusieurs fenêtres, les agence et, sous Stage Manager, les garde en groupe réaffichable.
- **Réglable** : une vraie fenêtre à treize onglets (Fenêtres, Calage, Dock, Groupes, Pendant le geste, Modificateurs, Clavier,
  Écrans, Exclusions, Général, Diagnostic, Mises à jour, À propos), au clavier avec ⌘1 à ⌘9, pour changer l'action de chaque
  geste en images, la sensibilité, la marge, les touches, les écrans et les apps exclues.
- **Sans conflit** : sous le geste, le défilement et les balayages du système (Mission Control, Spaces) sont retenus ; en dehors
  d'une barre de titre, tout reste au système.

Version de test : Glisse lit le trackpad par une interface non documentée d'Apple, qu'un futur macOS peut modifier.
Ce dépôt ne contient que les versions à installer. Le code source n'est pas public.

## Ce qu'il faut

- un Mac à puce Apple (M1 ou plus récent) avec un trackpad ;
- macOS 14 ou plus.

Aucun compte GitHub, aucun outil à installer, aucun mot de passe administrateur.

## Installer

Dans Terminal (Cmd + Espace, « Terminal »), une seule commande, qui installe aussi les mises à jour :

```
curl -fsSL https://raw.githubusercontent.com/LucasHRCHatReply/glisse-releases/main/installer.sh | zsh
```

Puis, une seule fois : Réglages Système › Confidentialité et sécurité › Accessibilité › activer « Glisse ».
Quittez les autres apps de gestes avant d'essayer.

## Mettre à jour

Fenêtre de Glisse (menu de la main › « Ouvrir Glisse… ») › onglet « Mises à jour » (Glisse vérifie aussi seule au démarrage, au plus une fois par jour),
ou relancer la commande ci-dessus. Les réglages sont conservés.

## Désinstaller

`~/Library/Application Support/Glisse/uninstall.sh` (posé par l'installation ; aussi dans le zip des Releases) :
il retire l'ouverture à la connexion, supprime l'app, retire l'autorisation Accessibilité si le système le permet,
et demande avant de supprimer les réglages.

## Version

0.7.1. Notes : voir la page des Releases.
