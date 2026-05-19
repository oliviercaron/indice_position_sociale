# Indice de Position Sociale (IPS) des établissements scolaires français

Exploration interactive des données IPS publiées par la DEPP (Direction de l'évaluation, de la prospective et de la performance) pour **129 046 établissements** scolaires français (écoles, collèges, lycées) sur la période 2022-2026.

## Applications

| Application | Description |
|---|---|
| [**Explorateur IPS**](https://oliviercaron.github.io/indice_position_sociale/) | Tableau interactif avec filtres, tri, recherche et export CSV/Excel |
| [Rapport IPS](https://oliviercaron.github.io/indice_position_sociale/rapport_ips.html) | 14 visualisations Chart.js avec analyses |

## Fonctionnalités de l'explorateur

- Filtres par type d'établissement, secteur, académie, rentrée scolaire, plage IPS
- Recherche textuelle (nom, commune, UAI)
- Tri ascendant/descendant sur toutes les colonnes
- Coloration de l'IPS pondérée par la distribution statistique (percentiles)
- Export de la sélection en CSV ou Excel
- Virtual scroll pour des performances optimales sur 129k lignes

## Données

Les données IPS proviennent de [data.education.gouv.fr](https://data.education.gouv.fr) et sont croisées avec le référentiel géographique des établissements.

| Fichier | Description |
|---|---|
| `data/ips_etablissements_geolocalises.parquet` | Données traitées (129 046 lignes, 10 colonnes) |
| `data/fr-en-adresse-et-geolocalisation-etablissements-premier-et-second-degre.parquet` | Référentiel géographique |

Les fichiers CSV sources (écoles, collèges, lycées) ne sont pas inclus dans le dépôt (>100 Mo). Ils sont téléchargeables sur [data.education.gouv.fr](https://data.education.gouv.fr/explore/dataset/fr-en-ips-ecoles-ap2022/) et [data.education.gouv.fr](https://data.education.gouv.fr/explore/dataset/fr-en-ips-colleges-ap2023/).
