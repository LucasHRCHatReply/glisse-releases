# Glisse pour macOS

Glisse ajoute une couche de gestes à la barre de titre des fenêtres : deux ou trois doigts qui glissent ou pincent sur
une barre de titre calent la fenêtre (moitié, tiers, agrandie, centrée), la passent en plein écran, la minimisent ou la
ferment. L'app vit dans la barre des menus (petite main). Aucun compte, aucune licence, aucune télémétrie.

- **Calage** : 2 doigts, glisser à gauche ou à droite = moitié de l'écran ; vers le haut = agrandir ; vers le bas = centrer.
- **Tiers** : 3 doigts, glisser à gauche, à droite ou vers le haut = tiers gauche, droit ou central.
- **Fenêtre** : 2 doigts écartés = plein écran ; pincés = minimiser ; 3 doigts pincés = fermer.
- **Réglable** : une vraie fenêtre à onglets (Gestes, Calage, Général, Mises à jour) pour changer l'action de chaque geste, la sensibilité, la marge et la hauteur de la barre de titre.
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

`uninstall.sh`, dans le dossier du zip téléchargé depuis la page des Releases.
