# W-Helper

Un petit panneau de contrôle pour Windows, pensé pour jouer : modes de performance, carte graphique, fréquence d'écran, rendu d'image, pilotes et nettoyage de la mémoire, en un clic. Il fonctionne sur n'importe quel PC, portable ou fixe, quelle que soit la marque.

<img src="panneau.png" alt="Le panneau W-Helper" width="282">

**[Télécharger W-Helper.exe](https://github.com/badb0ol/W-Helper/releases/latest/download/W-Helper.exe)**

Un seul fichier d'environ 150 Ko. Rien à installer, aucun droit administrateur, aucun service en arrière-plan.

## Démarrer

1. Téléchargez `W-Helper.exe` et lancez-le.
2. Windows affiche « Windows a protégé votre ordinateur » : l'application n'est pas encore signée. Cliquez sur **Informations complémentaires**, puis **Exécuter quand même**.
3. Au premier lancement, choisissez la touche qui affichera le panneau (par exemple `Ctrl+Alt+W`). Vous pouvez la changer à tout moment en cliquant dessus en bas du panneau.

Le panneau s'ouvre en bas à droite de l'écran, au-dessus des autres fenêtres. La croix le range dans la zone de notification ; votre touche ou un clic sur l'icône le fait revenir.

## Ce que fait le panneau

| Section | Ce que ça change |
|---|---|
| **Mesures** | Charge du processeur, de la mémoire et de la carte graphique |
| **Performance** | Silence, Équilibré ou Turbo : mode d'alimentation de Windows et boost du processeur |
| **Carte graphique** | Silence (60 images/s), Équilibré (réglages du pilote) ou Turbo, avec une carte NVIDIA ou AMD |
| **Écran** | Fréquence d'affichage, parmi celles que l'écran propose |
| **Image** | Standard, Jeu (ombres éclaircies), Film et Nuit (couleurs plus chaudes) |
| **Arrière-plan** | Liste des applications qui tournent en fond ; vous cochez celles à fermer |
| **Pilotes** | Pilotes installés et mises à jour proposées par Windows Update |
| **Audit** | Vérifie les oublis classiques : profil mémoire XMP/EXPO, écran sous sa fréquence maximale, écran branché sur la carte mère, etc. |

## Bon à savoir

- **Rien ne se ferme sans votre accord.** Le bouton Arrière-plan ouvre une liste ; seules les applications cochées sont fermées, et jamais une application dont la fenêtre est ouverte à l'écran.
- **Carte graphique.** Les modes fonctionnent avec les cartes NVIDIA et AMD (pilote Adrenalin récent). Turbo privilégie les performances maximales chez NVIDIA et active Radeon Anti-Lag chez AMD. Les cartes Intel ne sont pas encore prises en charge.
- **Pilotes.** « À jour » signifie que Windows Update ne propose rien de plus récent. Le fabricant peut publier une version plus récente sur son site ; un pilote graphique de plus d'un an est signalé avec le lien vers cette page.
- **Températures et ventilateurs** ne sont pas affichés : les lire demande un pilote système, que W-Helper n'installe pas.
- **Vie privée.** W-Helper n'envoie rien. La seule connexion est celle de Windows Update, quand la page Pilotes interroge le service de Windows.
- Vos choix sont gardés dans `%AppData%\W-Helper\settings.json`.

## Configuration requise

Windows 10 ou 11, 64 bits. Le .NET Framework 4.8 nécessaire est déjà présent sur ces versions de Windows.

## Licence

W-Helper est un logiciel propriétaire, distribué gratuitement. Voir [LICENSE.md](LICENSE.md).
