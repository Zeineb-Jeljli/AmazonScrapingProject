# AmazonScrapingProject : Analyse des données d'ordinateurs portables et tablettes

## Aperçu
Ce projet académique, réalisé entre le 04/09/2024 et le 25/11/2024, consiste à scraper des données sur les ordinateurs portables et tablettes disponibles sur Amazon, nettoyer ces données, et analyser les prix et caractéristiques pour identifier des tendances.

## Détails du projet
- **Objectif** : Collecter des données (titres, prix, évaluations, caractéristiques) sur les ordinateurs portables et tablettes, nettoyer les données, et analyser les tendances.
- **Source de données** : Site web d'Amazon (3 premières pages de résultats).
- **Outils utilisés** :
  - R avec les bibliothèques `rvest` (scraping), `dplyr`, `tidyr` (manipulation des données), `ggplot2`, `plotly` (visualisation).
  - Nettoyage des données : gestion des outliers (méthode IQR), imputation des valeurs manquantes (moyenne).

## Structure du dépôt
- `amazon_scraper.R` : Script R contenant le code de scraping et de nettoyage des données.
- `my_products.csv` : Fichier CSV avec les données brutes collectées.
- `cleaned_my_products.csv` : Fichier CSV avec les données nettoyées.
- `notebook.ipynb` : Notebook Jupyter détaillant le projet complet, incluant le code de scraping, une visualisation interactive (Plotly) des prix et fonctionnalités, une analyse des résultats, une conclusion, et des références bibliographiques.

## Résultats
- Collecte de données sur 72 produits (ordinateurs portables et tablettes, ex. : Acer Gateway Chromebook 311, Google Pixel Tablet).
- Nettoyage des données : suppression des symboles "$", conversion des prix en numérique, élimination des outliers, imputation des valeurs manquantes.
- Visualisation : graphique Plotly montrant les prix en fonction du nombre de fonctionnalités.
- Analyse : identification du produit avec le plus de fonctionnalités à bas prix (< 200$) : **Acer Gateway Chromebook 311 CBO311-1H-C1MX** à 159,90$.

## Améliorations futures
- Intégrer une visualisation interactive avec R Shiny pour explorer les données de manière dynamique.
- Étendre le scraping à d’autres catégories de produits (ex. : smartphones, livres).
