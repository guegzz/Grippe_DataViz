# Jeux de données utilisés

## Données géographiques

Afin de représenter les différents départements de France métropolitaine, nous utilisons un fichier GeoJSON <a href="https://github.com/ArnaudBru/ProjetBAC/blob/master/data/departements.geojson">departements.geojson</a> obtenu via le GitHub de <a href="https://github.com/gregoiredavid">Gregoire David</a>.
Ce fichier contient chacun des départements de France Métropolitaine. Il est organisé de la façon suivante

	{
		"type":"FeatureCollection",
		"features":[{
			"type":"Feature",
			"geometry":{
				"type":"Polygon",
				"coordinates":[[[3.172704,50.011997],[3.182198,50.012336],[3.205139,50.01835],[3.24521,50.02812],[3.257914,50.024437],
				...
				,[3.002756,49.218836],[2.997742,49.223581],[2.986693,49.218745],[2.985455,49.213082],[2.990226,49.210675]]]
			},
			"properties":{
				"code":"02",
				"nom":"Aisne"
			}
		},
		{
			"type":"Feature",
			"geometry":{
				"type":"Polygon",
				"coordinates":[[[3.414789,48.390269],[3.416604,48.399073],[3.422079,48.413341],[3.419746,48.416486],[3.413623,48.41434],
				...
				,[3.433818,48.361626],[3.427509,48.359976],[3.423838,48.365144],[3.421681,48.371728],[3.413273,48.376301],[3.414789,48.390269]]]
			},
			"properties":{
				"code":"10",
        "nom":"Aube"
			}
		},

		...

	}
  
Chaque feature représente ici un département, elle contient notamment un polygone qui représente les contours du département stockés sous forme d'une liste de points. Pour chacun des départements, on trouve deux propriétés, le nom du département ainsi que son code.

#### Récapitulatif technique

Type du fichier: Fichier GEOJSON (.geojson)

Taille: 1,03 Mo

Source: <a href="https://github.com/gregoiredavid/france-geojson">France Geojson</a>

## Données statistiques

Les données statistiques des résultats du Baccalauréat 2016 sont issues du <a href="https://www.data.gouv.fr/fr/">portail open data</a> du gouvernement français. Elles représentent les résultats des lycées d'enseignement général et technologique par filière en effectif et en taux. Le jeu de données est contenu dans un fichier excel (.xlsx)

Parmi les différents groupes de données du fichier, seuls trois nous intéressent.

### Informations générales

Les premières colonnes du fichier contiennent des informations générales concernant les établissements à savoir. Dans le cadre de notre étude, les données intéressantes sont:
- le code établissement qui nous sert de clé
- le nom de l'établissement pour d'éventuelles vérifications
- le code commune pour agréger les résultats par département
- le secteur, public ou privé

<img src="/img/data/Data_Infos_Generales.PNG" width=80% />

### Effectifs

Le deuxième groupe de données présent dans le fichier représente le nombre d'élèves à passer le bac par filière.

<img src="/img/data/Data_Effectifs.PNG" width=80% />

### Taux de réussite

Le troisième groupe de données présent dans le fichier représente le pourcentage d'élèves ayant obtenu le bac par filière.

<img src="/img/data/Data_Taux.PNG" width=80% />

#### Récapitulatif technique

Type du fichier: Feuille de calcul Microsoft Excel (.xlsx)

Taille: 651 Ko

Source: <a href="https://www.data.gouv.fr/fr/datasets/indicateurs-de-resultat-des-lycees-denseignement-general-et-technologique/#">data.gouv.fr</a>
