# licence.thibaultsan.com

Page unique qui publie les conditions d'utilisation de mes photographies, pour servir d'adresse stable dans :

- les métadonnées des fichiers exportés (champ `WebStatement` et mention de droits) ;
- les mentions de licence des sites qui publient mes photos (congrès REMPART, terre-chanvre, Seigneurie, tour-musée, site photo) ;
- les albums partagés et les messages sur Discord.

Source de référence, tenue dans mes notes : `Notes/Photo/activite/devis/TEMPLATE_CGU_photos_associatif.md`. En cas de divergence, c'est cette page publiée qui fait foi pour les tiers, puisque c'est elle qu'ils consultent.

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | Les conditions, en français, avec un résumé en anglais |
| `.well-known/tdmrep.json` | Réservation de fouille de textes et de données (protocole TDM Reservation) |
| `robots.txt` | Indexation autorisée, rappel de la réservation |
| `CNAME` | `licence.thibaultsan.com` |

## Mise en ligne

1. Créer le dépôt distant et pousser ce dossier.
2. Dans les réglages du dépôt, activer GitHub Pages sur la branche principale, à la racine.
3. Chez le gestionnaire du domaine, ajouter un enregistrement `CNAME` pour `licence` vers `<compte>.github.io`.
4. Vérifier que `https://licence.thibaultsan.com/.well-known/tdmrep.json` répond, certains hébergeurs filtrant les dossiers commençant par un point.

## Après la mise en ligne

Remplacer l'adresse provisoire `https://thibaultsan.com` par `https://licence.thibaultsan.com` dans :

- le préréglage Lightroom `Conditions Thibault Santonja 2026` (champ « URL des informations de copyright ») ;
- la variable `CONDITIONS` du script `Notes/Photo/activite/scripts/tatouer_metadonnees.sh`.

## Modifier les conditions

Toute modification ne vaut que pour l'avenir : les photographies déjà diffusées restent régies par la version en vigueur au moment de leur diffusion. Dater chaque version dans l'en-tête et le pied de page, et conserver l'historique dans git.
