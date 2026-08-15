# Version A — accueil éditorial (bandeau sombre + vignettes)

Site publié : https://athifexp-del.github.io/goldengroupci.github.io/

Ouvrir `index.html`. Cette version n'affiche que la direction visuelle **A** : le sélecteur de direction a été retiré.

## Remplacer une image

Écraser le fichier correspondant dans `images/` en gardant **exactement le même nom** (format JPG, 1400 px de large minimum, cadrage paysage sauf portraits de gouvernance). Aucune modification du HTML n'est nécessaire.

On peut aussi glisser-déposer une image directement sur un emplacement dans la page : le fichier déposé prend le dessus sur celui de `images/`.

| Fichier | Emplacement | Crédit photo (source) |
|---|---|---|
| `images/accueil-hero.jpg` | Accueil — visuel principal | [Photo by Omar on Unsplash](https://unsplash.com/@ommyjay) |
| `images/accueil-btp.jpg` | Accueil — vignette BTP | [Photo by Hammilton Ojijo on Unsplash](https://unsplash.com/@ojijohammilton) |
| `images/accueil-distribution.jpg` | Accueil — vignette Distribution | [Photo by Ali Mkumbwa on Unsplash](https://unsplash.com/@mkumbwajr) |
| `images/accueil-services.jpg` | Accueil — vignette Services numériques | [Photo by Ninthgrid on Unsplash](https://unsplash.com/@ninthgrid_) |
| `images/accueil-events.jpg` | Accueil — vignette Événementiel | [Photo by Ufoma Ojo on Unsplash](https://unsplash.com/@ladyufoma001) |
| `images/groupe-siege.jpg` | Page Le groupe — siège / équipe | [Photo by Kenrick Baksh on Unsplash](https://unsplash.com/@kenrick) |
| `images/pole-btp.jpg` | Pôle BTP & génie civil | [Photo by Mugabi Owen on Unsplash](https://unsplash.com/@spenz_official) |
| `images/pole-distribution.jpg` | Pôle Distribution audiovisuelle | [Photo by Ali Mkumbwa on Unsplash](https://unsplash.com/@mkumbwajr) |
| `images/pole-services.jpg` | Pôle Services numériques | [Photo by Emmanuel Ikwuegbu on Unsplash](https://unsplash.com/@emmages) |
| `images/pole-events.jpg` | Pôle Événementiel | [Photo by Andrea Qoqonga on Unsplash](https://unsplash.com/@filmmakerandrea6) |
| `images/carrieres-equipe.jpg` | Page Carrières — équipe au travail | [Photo by Ninthgrid on Unsplash](https://unsplash.com/@ninthgrid_) |

## Gouvernance

La section présente deux portraits :

| Poste | Nom | Photo |
|---|---|---|
| Président-directeur général | Koffi Tahi | `images/gouvernance-1.jpg` |
| Direction financière | Dohou Boris | `images/gouvernance-3.jpg` |

Les cadres sont en `aspect-ratio: 3 / 4` (format portrait) : le recadrage reste
identique quelle que soit la largeur d'écran, ce qui garantit que les visages
restent entiers. Ne pas remettre de `height` fixe sur ces `<figure>` — un cadre
paysage recoupe les têtes.

## Siège social

Le pied de page (présent sur toutes les pages) porte un bloc « Siège social »
avec une carte OpenStreetMap centrée sur les coordonnées du siège :

- **Coordonnées** : `5.371503, -3.968261`
- **Quartier** : Cocody — Bonoumin, Abidjan
- Le bouton « Itinéraire » ouvre Google Maps sur ces coordonnées.
- La carte est une iframe `openstreetmap.org/export/embed.html` en
  `loading="lazy"` : pas de clé d'API, pas de cookie de suivi, donc aucune
  bannière de consentement nécessaire. Le `bbox` encadre le point à ±0,0035°.

Pour déplacer le siège, mettre à jour au même endroit : le `bbox` et le
`marker` de l'iframe, le `destination` du lien Itinéraire, et les coordonnées
affichées en toutes lettres.

## Crédits

Photos de calage issues d'Unsplash (licence Unsplash : usage commercial autorisé, attribution non obligatoire). Les mentions en filigrane ont été retirées des images ; les crédits sont conservés dans le tableau ci-dessus à titre de trace. Ces visuels sont des images de calage, à remplacer par les photos Golden Group.
