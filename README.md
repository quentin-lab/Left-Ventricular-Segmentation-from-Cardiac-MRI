# Left-Ventricular-Segmentation-from-Cardiac-MRI

En se basant sur des techniques d'analyse d'image traditionnelle, et par opposition aux approches plus récente de Deep-Learning (type CNN), l'objectif de notre projet est de fournir une méthode de segmentation du ventricule gauche du coeur sur des images IRM. Cette méthode doit être robuste, précise et rapide.

## Plannification:
Pour mener à bien ce projet et sur les conseils de notre encadrant, nous avons décidé de nous concentrer sur un algorithme de segmentation par croissance de région.
Essentiellement, cela consiste à suivre les étapes suivantes:
1. **Choix de graine** (*seed finding*): choisir un pixel de départ le plus proche possible du centre du ventricule gauche.
2. **Segmentation par croissance de région**: (*region growing*) à partir de la graine, on va agrandir la région selon un critère.

## Jeu de données:
Notre jeu de données provient du [*Automatic Cardiac Diagnosis Challenge*](Automated Cardiac Diagnosis Challenge) organisé en 2017. Il est composé des images 4D (3d + temps) de 150 patients (100 pour l'entraînement et 50 pour le test). Pour chaque patient, des segmentations manuelles du ventricule gauche pour le moment de la pression maximale (systole) et de la pression minimale (diastole) sont fournies.
