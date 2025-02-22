Défi Open Data University - Diagnostics des Performances Energétiques - Niveau Confirmé

Analyse des Consommations Énergétiques et du DPE à Abbeville

Projet d'analyse des performances énergétiques des logements à Abbeville

Données : Open Data Enedis & Ademe

Technologies utilisées : Python, Pandas, Matplotlib, Seaborn, Scikit-learn

    Objectif du Projet
L’objectif de ce projet est d’évaluer l’impact de la classe de Diagnostic de Performance Énergétique (DPE) sur la consommation réelle d’électricité des logements à Abbeville.

Il s’agit de :
Comparer les estimations du DPE avec les consommations réelles issues des données Enedis.
Identifier les facteurs influençant la consommation énergétique : isolation, surface, type de chauffage, etc.
Visualiser les tendances et interpréter les écarts entre théorie et réalité.

        Structure du Projet

    Données sources :

dpe-v2-logements-existants.csv → Données des DPE des logements existants (source Ademe).
consommation-annuelle-residentielle-par-adresse.csv → Données de consommation énergétique par adresse (source Enedis).
donnees_abbeville.csv → Données filtrées pour Abbeville.
donnees_2023.csv → Données spécifiques pour Abbeville en 2023.

    Notebooks d’analyse :
    
  Préparation des données (préparation-données-dpe-abbeville.ipynb)

Filtrage des données DPE et Enedis pour Abbeville.
Normalisation et fusion des adresses.
Filtrage sur Abbeville, puis sur l’année 2023.

  Analyse des consommations pour 2023 (prédictions-dpe-abbeville-2023.ipynb)

Étude des consommations réelles des logements pour 2023.
Visualisation des tendances par classe DPE.
Premières prédictions et étude de la pertinence des variables.

  Analyse globale sans filtre temporel (prédictions-dpe-abbeville.ipynb)

    Résumé des Résultats

 Le type d’énergie principale de chauffage est le facteur le plus influent sur la consommation d’énergie.
 Les déperditions thermiques et la qualité de l’isolation jouent un rôle clé.
 La surface habitable a un fort impact sur la consommation;

Les analyses détaillées et interprétations sont disponibles dans les notebooks.
Ceci est un projet de niveau confirmé, bien que je sois encore débutante, il permet de pratique les différentes étapes d'un projet d'analyse de données: préparation de données, analyse exploratoire, prédictions.

    Comment Utiliser ce Projet:

1) Cloner le projet sur ton ordinateur
bash
Copier
Modifier
git clone https://github.com/TonNomGitHub/analyse_DPE_Abbeville.git
cd analyse_DPE_Abbeville

2) Installer les bibliothèques nécessaires:
bash
Copier
Modifier
pip install -r requirements.txt

3) Ouvrir et exécuter les notebooks Jupyter:
bash
Copier
Modifier
jupyter notebook

        Améliorations Possibles

Ce projet peut être amélioré en :
Ajoutant d’autres modèles de prédiction pour mieux expliquer les écarts DPE/consommation.
Testant des méthodes de sélection de variables pour optimiser les prédictions.
Enrichissant la base de données avec d’autres sources d’information (météo, équipements, etc.).


Auteur : Basak Basbunar






