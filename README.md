# Kmeans_Nabil_Ayoub
BIG DATA Project


## Projet clustering en K-Means:


# Objectif :

Notre objectif est d'agréger des emplacements des stations de vélos à l'aide de l'algorithme KMeans et de créer des clusters. 

Ce projet contient les documents suivants :

* Le dossier Code contient le code en python ;
* Le dossier Data contient la base de données de Brisbane-City-Bike ;
* Le dossier Exported comporte un fichier Excel des résultats du clustering ;
* le fichier Properties.conf contient les raccourcis des fichiers utilisés ;
* Le Readme qui décrit notre objectif, le déroulement du projet et les résultats obtenus ;

# La base de données :

La base de données (Bristol-city-bike.json) contient l’emplacement des vélos à Bristol. 

| address            | latitude | longitude| name	              | number |
|--------------------|----------|----------|--------------------|--------|
|Lower River Tce /...|-27.482279|153.028723|122 - LOWER RIVER...|	  122  |
|Main St / Darragh St| -27.47059|153.036046|91 - MAIN ST / DA...|    91  |
|Sydney St Ferry T...|-27.474531|153.042728|88 - SYDNEY ST FE...|    88  |

Elle est composée de 5 variables : 

* adresse : adresse de l'emplacement du vélo.
* latitude : latitude de l'emplacement du vélo 
* longitude : longitude de l'emplacement du vélo
* name : Le nombre et l'adresse du vélo
* number : numéro du vélo 

# Résultat du K-means

Le but est de faire une classification des vélos en tenant compte de leur situation géographique. Ainsi, nous avons décidé de ne conserver que les variables de latitude et de longitude comme variables d'entrée pour réaliser l'agrégation.
Les résultats de clustering ont permis de conclure qu'il existe 3 clusters :
Le premier groupe est à l'est, le deuxième groupe est au milieu et le troisième groupe est à l'ouest 

|Cluster   |       moy_latitude|     moy_longitude|
|----------|-------------------|------------------|
|EST       |-27.460240636363633|153.04186302272726|
|CENTRE    | -27.47255990624999|   153.02594553125|
|Ouest     |-27.481218536585374|153.00572882926832|

Voici la map qui illustre nos résultats de clustering :

![carte](https://user-images.githubusercontent.com/92821366/152610495-307fc591-b30f-4e72-9c00-ef8a72b293d0.PNG)



