# Préparation des données

## Données géographiques

Le fichier geojson contenant les données géographiques étant complet et propre, nous l'utiliserons tel quel, sans traitement.

## Données statistiques 

Toutes les colonnes du fichier ne nous intéressant pas, nous ne sélectionnons que les colonnes mentionnées dans <a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/DATA.MD">DATA.MD</a>
Une fois les colonnes récupérées, nous allons réorganiser les données afin qu'une ligne représente les effectifs et résultats d'une filière d'un établissement. En outre, nous allons modifier le format et utiliserons un format .csv plus universel et plus pratique d'utilisation.

L'établissement suivant ne possède des candidats que dans les filières S, ES et L

<img src="/img/data/Data_Exemple.PNG" width=80% />

Il sera donc lié à quatre lignes dans notre csv post-traitement (3 pour les différentes filières + 1 pour les résultats globaux)
Par ailleurs, à partir de la donnée "Code_Commune", on extrait le numéro de département de sorte que l'on obtient la structure finale suivante:

<img src="/img/data/Data_csv2.PNG" width=80% /> 

Les deux jeux de données sont ensuite liés dans le code JavaScript.
